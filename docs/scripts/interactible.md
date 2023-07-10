---
layout: default
title: Interactible
parent: Scripts
nav_order: 2
---
Enables different hand and pointer interactions when attached to a gameObject.

#### Global Variables

    class InteractibleEvent : UnityEvent<BaseInteractor> {}  
    enum HandGrabType

#### Public Members  

    public bool isLaserable
    public HandGrabType handGrabType

#### Hand-based Events
    
    InteractibleEvent OnTouch
    InteractibleEvent OffTouch
    InteractibleEvent OnGrab
    InteractibleEvent OffGrab

#### Pointer-based Events

    InteractibleEvent OnPointerOver
    InteractibleEvent OnPointerExit
    InteractibleEvent OnPointerClick
    InteractibleEvent OnPointerUnclick

#### Public Member Functions

    bool TryGrab(Interactor interactor, HandGrabType grabType)
    bool TryUngrab(Interactor interactor, HandGrabType grabType)

#### Private Member Functions

    void Start()