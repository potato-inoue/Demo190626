# Ins error of taco2.v2

<img src="img/CER_eval_same_feature.png" >

## Original results

| Acoustic model | Vocoder | Snt | Wrd | Corr | Sub | Del | Ins | Err | S.Err |  
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |  
| tacotron2.v2 | GL      | 250 | 21532 | 98.7 | 0.4 | 0.9 | 0.7 | 2.0 | 43.6 |  
| tacotron2.v2 | WNV_mol | 250 | 21532 | 98.6 | 0.4 | 1.0 | 3.6 | 5.0 | 42.8 |  
| tacotron2.v2 | WNV_nsf | 250 | 21532 | 99.0 | 0.4 | 0.6 | 3.7 | 4.7 | 38.4 |  
| tacotron2.v3 | GL      | 250 | 21532 | 98.5 | 0.5 | 0.9 | 0.4 | 1.8 | 45.2 |  


## After removing LJ050_0063 (Repetition example).

| Acoustic model | Vocoder | Snt | Wrd | Corr | Sub | Del | Ins | Err | S.Err |  
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |  
| tacotron2.v2 | GL      | 250 | 21532 | 98.7 | 0.4 | 0.9 | <font color="Red">0.3</font> | <font color="Red">1.6</font> | 43.6 |  
| tacotron2.v2 | WNV_mol | 250 | 21532 | 98.6 | 0.4 | 1.0 | <font color="Red">0.3</font> | <font color="Red">1.7</font> | 42.8 |  
| tacotron2.v2 | WNV_nsf | 250 | 21532 | 99.0 | 0.4 | 0.6 | <font color="Red">0.3</font> | <font color="Red">1.3</font> | 38.4 |  
| tacotron2.v3 | GL      | 250 | 21532 | 98.5 | 0.5 | 0.9 | 0.4 | 1.8 | 45.2 |  


## ASR output

    tacotorn2.v2 GL
    id: (lj050_0063)
    Scores: (#C #S #D #I) 98 0 0 96
    REF:  a n d w h o h a v e b e e n i n v o l v e d i n b o m b i n g o r b o m b m a k i n g o r w h o s e p a s t c o n d u c t i n d i c a t e s t e n d e n c i e s t o w a r d v i o l e n c e a n * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * d * * * * * * d * * * * 
    HYP:  a n d w h o h a v e b e e n i n v o l v e d i n b o m b i n g o r b o m b m a k i n g o r w h o s e p a s t c o n d u c t i n d i c a t e s t e n d e n c i e s t o w a r d v i o l e n c e a n D T O T H E D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O T H E D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O d E I T Y T O d E I T Y 
    Eval:                                                                                                                                                                                                 I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I   I I I I I I   I I I I 
      
    tacotorn2.v2 wnv_mol
    id: (lj050_0063)
    Scores: (#C #S #D #I) 98 0 0 721
    REF:  a n d w h o h a v e b e e n i n v o l v e d i n b o m b i n g o r b o m b m a k i n g o r w h o s e p a s t c o n d u c t i n d i c a t e s t e n d e n c i e s t o w a r d v i o l e n c e a n * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * 
    HYP:  a n d w h o h a v e b e e n i n v o l v e d i n b o m b i n g o r b o m b m a k i n g o r w h o s e p a s t c o n d u c t i n d i c a t e s t e n d e n c i e s t o w a r d v i o l e n c e a n D T O T H E D E I T Y T O D E I T Y T O D E I T Y T O T H E D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T 
    Eval:                                                                                                                                                                                                 I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I 
      
    >> REF:  * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * d * * * * * * d * * * * * * 
    >> HYP:  O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O d E I T Y T O d E I T Y T O 
    >> Eval: I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I   I I I I I I   I I I I I I 
      
    tacotorn2.v2 wnv_nsf
    id: (lj050_0063)
    Scores: (#C #S #D #I) 98 0 0 723
    REF:  a n d w h o h a v e b e e n i n v o l v e d i n b o m b i n g o r b o m b m a k i n g o r w h o s e p a s t c o n d u c t i n d i c a t e s t e n d e n c i e s t o w a r d v i o l e n c e a n * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * 
    HYP:  a n d w h o h a v e b e e n i n v o l v e d i n b o m b i n g o r b o m b m a k i n g o r w h o s e p a s t c o n d u c t i n d i c a t e s t e n d e n c i e s t o w a r d v i o l e n c e a n D T O T H E D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O T H E D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T O D E I T Y T 
    Eval:                                                                                                                                                                                                 I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I I 


## wav

| type | wav |  
| --- | --- |  
| GL v2      | <audio src="ins_taco2.v2/tacotron2.v2.GL/LJ050-0063.wav" controls></audio> |  
| WNV_mol v2 | <audio src="ins_taco2.v2/tacotron2.v2.wnv_mol/LJ050-0063_gen.wav" controls></audio> |  
| WNV_nsf v2 | <audio src="ins_taco2.v2/tacotron2.v2.wnv_nsf/LJ050-0063.wav" controls></audio> |  
| GL v3      | <audio src="ins_taco2.v2/tacotron2.v2.wnv_nsf/LJ050-0063.wav" controls></audio> |  


## att_ws of end2end ASR

### GL v2
<img src="ins_taco2.v2/tacotron2.v2.GL/LJ050-0063_att_ws_gl.png" width="640px">  

### WNV_mol v2
<img src="ins_taco2.v2/tacotron2.v2.wnv_mol/LJ050-0063_att_ws_wnv_mol.png" width="640px">  

### WNV_nsf v2
<img src="ins_taco2.v2/tacotron2.v2.wnv_nsf/LJ050-0063_att_ws_wnv_nsf.png" width="640px">  

### GL v3
<img src="ins_taco2.v2/tacotron2.v3.GL/LJ050-0063_att_ws.png" width="640px">  

## tacotron2.v3

Repetition was sloved in v3.  

    tacotorn2.v3 GL
    id: (lj050_0063)
    Scores: (#C #S #D #I) 98 0 0 0
    REF:  a n d w h o h a v e b e e n i n v o l v e d i n b o m b i n g o r b o m b m a k i n g o r w h o s e p a s t c o n d u c t i n d i c a t e s t e n d e n c i e s t o w a r d v i o l e n c e a n d d 
    HYP:  a n d w h o h a v e b e e n i n v o l v e d i n b o m b i n g o r b o m b m a k i n g o r w h o s e p a s t c o n d u c t i n d i c a t e s t e n d e n c i e s t o w a r d v i o l e n c e a n d d 
    Eval:                                                                                                                                                                                                     
      
    tacotorn2.v3 wnv_mol
    id: (lj050_0063)
    Scores: (#C #S #D #I) 95 0 3 0
    REF:  A N D w h o h a v e b e e n i n v o l v e d i n b o m b i n g o r b o m b m a k i n g o r w h o s e p a s t c o n d u c t i n d i c a t e s t e n d e n c i e s t o w a r d v i o l e n c e a n d d 
    HYP:  * * * w h o h a v e b e e n i n v o l v e d i n b o m b i n g o r b o m b m a k i n g o r w h o s e p a s t c o n d u c t i n d i c a t e s t e n d e n c i e s t o w a r d v i o l e n c e a n d d 
    Eval: D D D                                                                                                                                                                                               
      
    tacotorn2.v3 wnv_nsf
    id: (lj050_0063)
    Scores: (#C #S #D #I) 98 0 0 0
    REF:  a n d w h o h a v e b e e n i n v o l v e d i n b o m b i n g o r b o m b m a k i n g o r w h o s e p a s t c o n d u c t i n d i c a t e s t e n d e n c i e s t o w a r d v i o l e n c e a n d d 
    HYP:  a n d w h o h a v e b e e n i n v o l v e d i n b o m b i n g o r b o m b m a k i n g o r w h o s e p a s t c o n d u c t i n d i c a t e s t e n d e n c i e s t o w a r d v i o l e n c e a n d d 
    Eval:                                                                                                                                                                                                     
