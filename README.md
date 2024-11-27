# SkinSmoothing

In this proect you will perform skin smoothing on a face. If you smooth the entire face, the results would be terrible. Even if you use edge preserving filters like bilateral filter, results may not look very good. So we need to find skin region before performing smoothing.
Steps:
1. Use Face Detection to find face region or specific areas like cheek/forehead.
   Based on location of face, you can find location of cheek and forehead using some heuristics
2. Use skin pixels to build a color model for skin.
   You can apply this color model to entire face to detect skin
3. Perform smoothing only on these skin pixels
