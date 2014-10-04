---
layout: post
title: Day 21 - Completed camera control in C++
date: 2014-10-04
tags: [blog]
time: 45
---

I got UE4 to find the C++ method I made, and figured out how to write all the code in C++. Here it is:

{% highlight c++ %}
const int bufferSize = 100;
const int scrollSpeed = 1000;

FVector UCameraUtilityNode::GetNewCameraPosition(FVector OriginalCameraLoc, float DeltaTime, float MouseX, float MouseY)
{
	FVector translate = FVector(0.f, 0.f, 0.f);
	const FVector2D ViewportSize = FVector2D(GEngine->GameViewport->Viewport->GetSizeXY());

	// left/right
	if (MouseX <= bufferSize)
		translate.Y += scrollSpeed * DeltaTime;
	else if (MouseX >= ViewportSize.X - bufferSize)
		translate.Y -= scrollSpeed * DeltaTime;

	// up/down
	if (MouseY <= bufferSize)
		translate.X -= scrollSpeed * DeltaTime;
	else if (MouseY >= ViewportSize.Y - bufferSize)
		translate.X += scrollSpeed * DeltaTime;

	return OriginalCameraLoc + translate;
}
{% endhighlight %}