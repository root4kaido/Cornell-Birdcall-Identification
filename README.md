# Kaggle Competion

## Overview
https://www.kaggle.com/c/birdsong-recognition/overview

<img src="https://github.com/root4kaido/Cornell-Birdcall-Identification/blob/master/Material/bird.png" width=20%, align=right>

> In this competition, you will identify a wide variety of bird vocalizations in soundscape recordings. Due to the complexity of the recordings, they contain weak labels. There might be anthropogenic sounds (e.g., airplane overflights) or other bird and non-bird (e.g., chipmunk) calls in the background, with a particular labeled bird species in the foreground. Bring your new ideas to build effective detectors and classifiers for analyzing complex soundscape recordings!

## Try
- event+random crop
- randoms crop
- mask inference
- class balanced training
- mixup
- add gaussian noise
- ensemble
- choice duration 
- choice rating

## Findings

### inference
- maskして走査はききそう→分類にはきくけど，nocallのせいでダメ
- nocall のデータが半分を占めているので，優先度は，nocallの識別精度保持 > 鳥の分類精度向上

__本質は，鳥の分類より，no call / calll分類！！！！__

### training
- gausenoise追加はききそう→そうでもない
- mixupはききそう→そうでもない
- data選んだりはしないほうが良さそう
