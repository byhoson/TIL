# CSS RENDERING

 이 글은 code spitz 72의 css rendering 수업을 듣고 정리한 글이다.

## RENDERING SYSTEM

 Rendering 할 때에는 Document의 DOM 구조를 생각하지 않고 각각의 Element(BFC, IFC, RP)마다 별개로 그린다.
 순서는 다음과 같다.

1. Calculate Geometry
 Document의 전체적인 골격을 구성한다. (땅따먹기)

2. Fill Fragments
 Geometry를 토대로 Fragment를 칠한다. 여기서 Pixel을 칠한다고 표현하지 않은 이유는 Geometry에 따라 칠해야 할 영역의 
 크기가 바뀌기 때문.

## NORMAL FLOW

1. BFC (Box Formatting Contexts)
2. IFC (Inline Formatting Contexts)
3. RP (Relative Positioning)