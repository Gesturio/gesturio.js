# gesturio.js

Usage example on coffee script

```
Gesture.GesturesSet = GesturesSets.en

Leap.loop (frame) ->
  if frame.hands[0]
    Gesture.getGestureParams frame.hands[0]
    params = Gesture.getParamsArray()
    Gesture.getMetrics params
    decision = Gesture.makeDecision()
    console.log decision

```