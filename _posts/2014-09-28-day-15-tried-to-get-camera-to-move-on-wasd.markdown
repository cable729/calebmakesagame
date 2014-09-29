---
layout: post
title: Day 15 - Tried to get camera to move on WASD
date: 2014-09-28
tags: [blog]
time: 60
---

I tried to get the camera to move, still confused with all the inner working. Here's my current code for a tick:

    void AMazeBasicalisPlayerController::PlayerTick(float DeltaTime)
    {
        APawn* camera = GetControlledPawn();
        camera->SetActorRelativeLocation(direction);
    }

No matter how I try to move the game component, it doesn't go.