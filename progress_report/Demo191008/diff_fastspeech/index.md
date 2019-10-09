# Del error of fastspeech

<img src="../img/CER_eval_same_feature.png" >

## Original results

| Acoustic model | Vocoder | Snt | Wrd | Corr | Sub | Del | Ins | Err | S.Err |  
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |  
| fastspeech.v1 | GL | 250 | 21532 | 98.3 | 0.4 | 1.3 | 0.4 | 2.1 | 44.4 |  
| fastspeech.v2 | GL | 250 | 21532 | 98.7 | 0.4 | 0.9 | 0.3 | 1.6 | 41.2 |  

## Deletion of "The"

### ASR output

    fastspeech.v1.gl
    id: (lj050_0030)
    Scores: (#C #S #D #I) 24 0 3 0
    REF:  T H E c o m m i s s i o n a l s o r e c o m m e n d s 
    HYP:  * * * c o m m i s s i o n a l s o r e c o m m e n d s 
    Eval: D D D                                                 
    ----
    fastspeech.v2.gl
    id: (lj050_0030)
    Scores: (#C #S #D #I) 27 0 0 0
    REF:  t h e c o m m i s s i o n a l s o r e c o m m e n d s 
    HYP:  t h e c o m m i s s i o n a l s o r e c o m m e n d s 
    Eval:                                                       

### wav

| type | wav |  
| --- | --- |  
| fastspeech v1 | <audio src="fastspeech.v1.gl/LJ050-0030.wav" controls></audio> |  
| fastspeech v2 | <audio src="fastspeech.v2.gl/LJ050-0030.wav" controls></audio> |  

### ASR output

    fastspeech.v1.gl
    id: (lj050_0269)
    Scores: (#C #S #D #I) 63 1 5 1
    REF:  T H E e s s e n t i a l t e r m s o f s u c h m e m o r a n d * A m i g h t w e l l b e e m b o d i e d i N A n e x e c u t i v e o r d e r 
    HYP:  * * * e s s e n t i a l t e r m s o f s u c h m e m o r a n d U M m i g h t w e l l b e e m b o d i e d i * * n e x e c u t i v e o r d e r 
    Eval: D D D                                                         I S                                         D D                               
    ----
    fastspeech.v2.gl
    id: (lj050_0269)
    Scores: (#C #S #D #I) 68 1 0 1
    REF:  t h e e s s e n t i a l t e r m s o f s u c h m e m o r a n d * A m i g h t w e l l b e e m b o d i e d i n a n e x e c u t i v e o r d e r 
    HYP:  t h e e s s e n t i a l t e r m s o f s u c h m e m o r a n d U M m i g h t w e l l b e e m b o d i e d i n a n e x e c u t i v e o r d e r 
    Eval:                                                               I S                                                                           

| type | wav |  
| --- | --- |  
| fastspeech v1 | <audio src="fastspeech.v1.gl/LJ050-0269.wav" controls></audio> |  
| fastspeech v2 | <audio src="fastspeech.v2.gl/LJ050-0269.wav" controls></audio> |  

## Deletion of "And"

### ASR output

    fastspeech.v1.gl
    id: (lj050_0194)
    Scores: (#C #S #D #I) 86 0 3 0
    REF:  A N D s h o u l d n o t b e r e l i e d u p o n t o t h e d e t r i m e n t o f t h e i m a g i n a t i v e a p p l i c a t i o n o f j u d g m e n t i n s p e c i a l c a s e s 
    HYP:  * * * s h o u l d n o t b e r e l i e d u p o n t o t h e d e t r i m e n t o f t h e i m a g i n a t i v e a p p l i c a t i o n o f j u d g m e n t i n s p e c i a l c a s e s 
    Eval: D D D                                                                                                                                                                             
    ----
    fastspeech.v2.gl
    id: (lj050_0194)
    Scores: (#C #S #D #I) 89 0 0 0
    REF:  a n d s h o u l d n o t b e r e l i e d u p o n t o t h e d e t r i m e n t o f t h e i m a g i n a t i v e a p p l i c a t i o n o f j u d g m e n t i n s p e c i a l c a s e s 
    HYP:  a n d s h o u l d n o t b e r e l i e d u p o n t o t h e d e t r i m e n t o f t h e i m a g i n a t i v e a p p l i c a t i o n o f j u d g m e n t i n s p e c i a l c a s e s 
    Eval:                                                                                                                                                                                   

| type | wav |  
| --- | --- |  
| fastspeech v1 | <audio src="fastspeech.v1.gl/LJ050-0194.wav" controls></audio> |  
| fastspeech v2 | <audio src="fastspeech.v2.gl/LJ050-0194.wav" controls></audio> |  

### ASR output

    fastspeech.v1.gl
    id: (lj050_0225)
    Scores: (#C #S #D #I) 61 0 3 0
    REF:  A N D b e a v a i l a b l e t o p r o t e c t t h e p r e s i d e n t o r v i c e p r e s i d e n t w h e n t h e y t r a v e l 
    HYP:  * * * b e a v a i l a b l e t o p r o t e c t t h e p r e s i d e n t o r v i c e p r e s i d e n t w h e n t h e y t r a v e l 
    Eval: D D D                                                                                                                           
    ----
    fastspeech.v2.gl
    id: (lj050_0225)
    Scores: (#C #S #D #I) 64 0 0 0
    REF:  a n d b e a v a i l a b l e t o p r o t e c t t h e p r e s i d e n t o r v i c e p r e s i d e n t w h e n t h e y t r a v e l 
    HYP:  a n d b e a v a i l a b l e t o p r o t e c t t h e p r e s i d e n t o r v i c e p r e s i d e n t w h e n t h e y t r a v e l 
    Eval:                                                                                                                                 

| type | wav |  
| --- | --- |  
| fastspeech v1 | <audio src="fastspeech.v1.gl/LJ050-0225.wav" controls></audio> |  
| fastspeech v2 | <audio src="fastspeech.v2.gl/LJ050-0225.wav" controls></audio> |  


## Deletion of "With"

### ASR output

    fastspeech.v1.gl
    id: (lj050_0265)
    Scores: (#C #S #D #I) 130 0 4 0
    REF:  W I T H t h e o f f i c e o f s c i e n c e a n d t e c h n o l o g y a n d t h e o t h e r f e d e r a l a g e n c i e s t h a t h a v e b e e n s o h e l p f u l t o t h e s e c r e t s e r v i c e b e p l a c e d o n a p e r m a n e n t a n d f o r m a l b a s i s 
    HYP:  * * * * t h e o f f i c e o f s c i e n c e a n d t e c h n o l o g y a n d t h e o t h e r f e d e r a l a g e n c i e s t h a t h a v e b e e n s o h e l p f u l t o t h e s e c r e t s e r v i c e b e p l a c e d o n a p e r m a n e n t a n d f o r m a l b a s i s 
    Eval: D D D D                                                                                                                                                                                                                                                                     
    ----
    fastspeech.v2.gl
    id: (lj050_0265)
    Scores: (#C #S #D #I) 134 0 0 0
    REF:  w i t h t h e o f f i c e o f s c i e n c e a n d t e c h n o l o g y a n d t h e o t h e r f e d e r a l a g e n c i e s t h a t h a v e b e e n s o h e l p f u l t o t h e s e c r e t s e r v i c e b e p l a c e d o n a p e r m a n e n t a n d f o r m a l b a s i s 
    HYP:  w i t h t h e o f f i c e o f s c i e n c e a n d t e c h n o l o g y a n d t h e o t h e r f e d e r a l a g e n c i e s t h a t h a v e b e e n s o h e l p f u l t o t h e s e c r e t s e r v i c e b e p l a c e d o n a p e r m a n e n t a n d f o r m a l b a s i s 
    Eval:                                                                                                                                                                                                                                                                             

| type | wav |  
| --- | --- |  
| fastspeech v1 | <audio src="fastspeech.v1.gl/LJ050-0265.wav" controls></audio> |  
| fastspeech v2 | <audio src="fastspeech.v2.gl/LJ050-0265.wav" controls></audio> |  


### ASR output

    fastspeech.v1.gl
    id: (lj050_0277)
    Scores: (#C #S #D #I) 127 0 4 0
    REF:  W I T H t h e a c t i v e c o o p e r a t i o n o f t h e r e s p o n s i b l e a g e n c i e s a n d w i t h t h e u n d e r s t a n d i n g o f t h e p e o p l e o f t h e u n i t e d s t a t e s i n t h e i r d e m a n d s u p o n t h e i r p r e s i d e n t 
    HYP:  * * * * t h e a c t i v e c o o p e r a t i o n o f t h e r e s p o n s i b l e a g e n c i e s a n d w i t h t h e u n d e r s t a n d i n g o f t h e p e o p l e o f t h e u n i t e d s t a t e s i n t h e i r d e m a n d s u p o n t h e i r p r e s i d e n t 
    Eval: D D D D                                                                                                                                                                                                                                                               
    ----
    fastspeech.v2.gl
    id: (lj050_0277)
    Scores: (#C #S #D #I) 130 1 0 1
    REF:  w i t h t h e a c t i v e c o o p e r a t i o n o f t h e r e s p o n s i b l e a g e n c i e s a n d w i t h t h e u n d e r s t a n d i n g o f t h e p e o p l e o f t h e u n i t e d s t a t e s I n * t h e i r d e m a n d s u p o n t h e i r p r e s i d e n t 
    HYP:  w i t h t h e a c t i v e c o o p e r a t i o n o f t h e r e s p o n s i b l e a g e n c i e s a n d w i t h t h e u n d e r s t a n d i n g o f t h e p e o p l e o f t h e u n i t e d s t a t e s A n D t h e i r d e m a n d s u p o n t h e i r p r e s i d e n t 
    Eval:                                                                                                                                                                                                       S   I                                                             

| type | wav |  
| --- | --- |  
| fastspeech v1 | <audio src="fastspeech.v1.gl/LJ050-0277.wav" controls></audio> |  
| fastspeech v2 | <audio src="fastspeech.v2.gl/LJ050-0277.wav" controls></audio> |  


## Deletion of "In"

### ASR output

    fastspeech.v1.gl
    id: (lj050_0038)
    Scores: (#C #S #D #I) 70 0 2 0
    REF:  I N a t t e m p t i n g t o i d e n t i f y t h o s e i n d i v i d u a l s w h o m i g h t p r o v e a d a n g e r t o t h e p r e s i d e n t 
    HYP:  * * a t t e m p t i n g t o i d e n t i f y t h o s e i n d i v i d u a l s w h o m i g h t p r o v e a d a n g e r t o t h e p r e s i d e n t 
    Eval: D D                                                                                                                                             
    ----
    fastspeech.v2.gl
    id: (lj050_0038)
    Scores: (#C #S #D #I) 72 0 0 0
    REF:  i n a t t e m p t i n g t o i d e n t i f y t h o s e i n d i v i d u a l s w h o m i g h t p r o v e a d a n g e r t o t h e p r e s i d e n t 
    HYP:  i n a t t e m p t i n g t o i d e n t i f y t h o s e i n d i v i d u a l s w h o m i g h t p r o v e a d a n g e r t o t h e p r e s i d e n t 
    Eval:                                                                                                                                                 

| type | wav |  
| --- | --- |  
| fastspeech v1 | <audio src="fastspeech.v1.gl/LJ050-0038.wav" controls></audio> |  
| fastspeech v2 | <audio src="fastspeech.v2.gl/LJ050-0038.wav" controls></audio> |  


## Deletion of "guide"

### ASR output

    fastspeech.v1.gl
    id: (lj050_0079)
    Scores: (#C #S #D #I) 58 0 5 2
    REF:  G U I D E l i n e s f o r a n e x p e r i m e n t a l p r o g r a * m * t o d e v e l o p m o r e d e t a i l e d c r i t e r i a 
    HYP:  * * * * * l i n e s f o r a n e x p e r i m e n t a l p r o g r a M m E t o d e v e l o p m o r e d e t a i l e d c r i t e r i a 
    Eval: D D D D D                                                         I   I                                                           
    ----
    fastspeech.v2.gl
    id: (lj050_0079)
    Scores: (#C #S #D #I) 61 1 1 0
    REF:  G U i d e l i n e s f o r a n e x p e r i m e n t a l p r o g r a m t o d e v e l o p m o r e d e t a i l e d c r i t e r i a 
    HYP:  * S i d e l i n e s f o r a n e x p e r i m e n t a l p r o g r a m t o d e v e l o p m o r e d e t a i l e d c r i t e r i a 
    Eval: D S                                                                                                                           

| type | wav |  
| --- | --- |  
| fastspeech v1 | <audio src="fastspeech.v1.gl/LJ050-0079.wav" controls></audio> |  
| fastspeech v2 | <audio src="fastspeech.v2.gl/LJ050-0079.wav" controls></audio> |  


### ASR output

    fastspeech.v1.gl
    id: (lj050_0080)
    Scores: (#C #S #D #I) 64 1 7 2
    REF:  T H E s u g g e s t i o n s o f f e d e r a l a g e n c i e s f o R r E v i s i o n o f t h e s e G U I d e * * l i n e s w e r e s o l i c i t e d 
    HYP:  * * * s u g g e s t i o n s o f f e d e r a l a g e n c i e s f o * r A v i s i o n o f t h e s e * * * d e A D l i n e s w e r e s o l i c i t e d 
    Eval: D D D                                                             D   S                           D D D     I I                                     
    ----
    fastspeech.v2.gl
    id: (lj050_0080)
    Scores: (#C #S #D #I) 69 0 3 0
    REF:  T H E s u g g e s t i o n s o f f e d e r a l a g e n c i e s f o r r e v i s i o n o f t h e s e g u i d e l i n e s w e r e s o l i c i t e d 
    HYP:  * * * s u g g e s t i o n s o f f e d e r a l a g e n c i e s f o r r e v i s i o n o f t h e s e g u i d e l i n e s w e r e s o l i c i t e d 
    Eval: D D D                                                                                                                                           

| type | wav |  
| --- | --- |  
| fastspeech v1 | <audio src="fastspeech.v1.gl/LJ050-0080.wav" controls></audio> |  
| fastspeech v2 | <audio src="fastspeech.v2.gl/LJ050-0080.wav" controls></audio> |  


## Deletion of "Were"

### ASR output

    fastspeech.v1.gl
    id: (lj050_0103)
    Scores: (#C #S #D #I) 91 0 4 0
    REF:  W E R E a l l m e n w h o a c t e d a l o n e i n t h e i r c r i m i n a l a c t s a g a i n s t o u r l e a d e r s n o n e h a d a s e r i o u s r e c o r d o f p r i o r v i o l e n c e 
    HYP:  * * * * a l l m e n w h o a c t e d a l o n e i n t h e i r c r i m i n a l a c t s a g a i n s t o u r l e a d e r s n o n e h a d a s e r i o u s r e c o r d o f p r i o r v i o l e n c e 
    Eval: D D D D                                                                                                                                                                                       
    ----
    fastspeech.v2.gl
    id: (lj050_0103)
    Scores: (#C #S #D #I) 95 0 0 0
    REF:  w e r e a l l m e n w h o a c t e d a l o n e i n t h e i r c r i m i n a l a c t s a g a i n s t o u r l e a d e r s n o n e h a d a s e r i o u s r e c o r d o f p r i o r v i o l e n c e 
    HYP:  w e r e a l l m e n w h o a c t e d a l o n e i n t h e i r c r i m i n a l a c t s a g a i n s t o u r l e a d e r s n o n e h a d a s e r i o u s r e c o r d o f p r i o r v i o l e n c e 
    Eval:                                                                                                                                                                                               

| type | wav |  
| --- | --- |  
| fastspeech v1 | <audio src="fastspeech.v1.gl/LJ050-0103.wav" controls></audio> |  
| fastspeech v2 | <audio src="fastspeech.v2.gl/LJ050-0103.wav" controls></audio> |  


## Deletion of "This"

### ASR output

    fastspeech.v1.gl
    id: (lj050_0115)
    Scores: (#C #S #D #I) 43 0 6 0
    REF:  T H I S i s e s p e c i a l l y n e c e s s a r y w i t h r e g a r d t o t h e f b i a n d c I A 
    HYP:  * * * * i s e s p e c i a l l y n e c e s s a r y w i t h r e g a r d t o t h e f b i a n d c * * 
    Eval: D D D D                                                                                       D D 
    ----
    fastspeech.v2.gl
    id: (lj050_0115)
    Scores: (#C #S #D #I) 47 1 1 1
    REF:  t h i s i s e s p e c i a l l y n e c e s s a r y w i t h r e g a r d t o t h e f b i a n d C I a * 
    HYP:  t h i s i s e s p e c i a l l y n e c e s s a r y w i t h r e g a r d t o t h e f b i a n d * S a Y 
    Eval:                                                                                             D S   I 

| type | wav |  
| --- | --- |  
| fastspeech v1 | <audio src="fastspeech.v1.gl/LJ050-0115.wav" controls></audio> |  
| fastspeech v2 | <audio src="fastspeech.v2.gl/LJ050-0115.wav" controls></audio> |  


## Deletion of "They"

### ASR output

    fastspeech.v1.gl
    id: (lj050_0119)
    Scores: (#C #S #D #I) 110 0 4 0
    REF:  T H E Y s h o u l d b e r e s p o n s i b l e f o r a d v i s i n g t h e s e c r e t s e r v i c e i f i n f o r m a t i o n d e v e l o p s i n d i c a t i n g t h e e x i s t e n c e o f a n a s s a s s i n a t i o n p l o t 
    HYP:  * * * * s h o u l d b e r e s p o n s i b l e f o r a d v i s i n g t h e s e c r e t s e r v i c e i f i n f o r m a t i o n d e v e l o p s i n d i c a t i n g t h e e x i s t e n c e o f a n a s s a s s i n a t i o n p l o t 
    Eval: D D D D                                                                                                                                                                                                                             
    ----
    fastspeech.v2.gl
    id: (lj050_0119)
    Scores: (#C #S #D #I) 114 0 0 0
    REF:  t h e y s h o u l d b e r e s p o n s i b l e f o r a d v i s i n g t h e s e c r e t s e r v i c e i f i n f o r m a t i o n d e v e l o p s i n d i c a t i n g t h e e x i s t e n c e o f a n a s s a s s i n a t i o n p l o t 
    HYP:  t h e y s h o u l d b e r e s p o n s i b l e f o r a d v i s i n g t h e s e c r e t s e r v i c e i f i n f o r m a t i o n d e v e l o p s i n d i c a t i n g t h e e x i s t e n c e o f a n a s s a s s i n a t i o n p l o t 
    Eval:                                                                                                                                                                                                                                     

| type | wav |  
| --- | --- |  
| fastspeech v1 | <audio src="fastspeech.v1.gl/LJ050-0119.wav" controls></audio> |  
| fastspeech v2 | <audio src="fastspeech.v2.gl/LJ050-0119.wav" controls></audio> |  


## Deletion of "that"

### ASR output

    fastspeech.v1.gl
    id: (lj050_0179)
    Scores: (#C #S #D #I) 101 1 6 0
    REF:  b a s e d o n i t s e x p e r i e n c e d u r i n g t h i s p e r i o d t h e s e c r e t s e r v i c e n o w r e c o m m e n d s T H A T a d d i t i o n a l p e r s o N n E l b e m a d e a v a i l a b l e t o p R s 
    HYP:  b a s e d o n i t s e x p e r i e n c e d u r i n g t h i s p e r i o d t h e s e c r e t s e r v i c e n o w r e c o m m e n d s * * * * a d d i t i o n a l p e r s o * n A l b e m a d e a v a i l a b l e t o p * s 
    Eval:                                                                                                                                   D D D D                               D   S                                       D   
    ----
    fastspeech.v2.gl
    id: (lj050_0179)
    Scores: (#C #S #D #I) 107 1 0 4
    REF:  b a s e d o n i t s e x p e r i e n c e d u r i n g t h i s p e r i o d t h e s e c r e t s e r v i c e n o w r e c o m m e n d s t h a t a d d i t i o n a l p e r s o n n e l b e m a d e a v a i l a b l e t o * * * P r * s 
    HYP:  b a s e d o n i t s e x p e r i e n c e d u r i n g t h i s p e r i o d t h e s e c r e t s e r v i c e n o w r e c o m m e n d s t h a t a d d i t i o n a l p e r s o n n e l b e m a d e a v a i l a b l e t o C H I A r A s 
    Eval:                                                                                                                                                                                                                   I I I S   I   

| type | wav |  
| --- | --- |  
| fastspeech v1 | <audio src="fastspeech.v1.gl/LJ050-0179.wav" controls></audio> |  
| fastspeech v2 | <audio src="fastspeech.v2.gl/LJ050-0179.wav" controls></audio> |  


### ASR output

    fastspeech.v1.gl
    id: (lj050_0241)
    Scores: (#C #S #D #I) 63 0 9 0
    REF:  T H E f b i h a s i n d i c a t e d T H A T I T i s w i l l i n g t o c o n t i n u e t o m a k e s u c h a s s i s t a n c e a v a i l a b l e 
    HYP:  * * * f b i h a s i n d i c a t e d * * * * * * i s w i l l i n g t o c o n t i n u e t o m a k e s u c h a s s i s t a n c e a v a i l a b l e 
    Eval: D D D                               D D D D D D                                                                                                 
    ----
    fastspeech.v2.gl
    id: (lj050_0241)
    Scores: (#C #S #D #I) 69 0 3 0
    REF:  T H E f b i h a s i n d i c a t e d t h a t i t i s w i l l i n g t o c o n t i n u e t o m a k e s u c h a s s i s t a n c e a v a i l a b l e 
    HYP:  * * * f b i h a s i n d i c a t e d t h a t i t i s w i l l i n g t o c o n t i n u e t o m a k e s u c h a s s i s t a n c e a v a i l a b l e 
    Eval: D D D                                                                                                                                           

| type | wav |  
| --- | --- |  
| fastspeech v1 | <audio src="fastspeech.v1.gl/LJ050-0241.wav" controls></audio> |  
| fastspeech v2 | <audio src="fastspeech.v2.gl/LJ050-0241.wav" controls></audio> |  


## Complex example

### ASR output

    fastspeech.v1.gl
    id: (lj050_0060)
    Scores: (#C #S #D #I) 84 3 7 2
    REF:  s u b v e r s i v e s u l t r a R I G H t i s t s r A c * i s t s a n d f a s c i s t s * A p o s s e s s i n g e m o t i o n a l i n s t a b i l i t y O R I R r a t i o n a l b e h a v i o r 
    HYP:  s u b v e r s i v e s u l t r a * * * * t i s t s r I c E i s t s a n d f a s c i s t s O F p o s s e s s i n g e m o t i o n a l i n s t a b i l i t y * * * A r a t i o n a l b e h a v i o r 
    Eval:                                 D D D D             S   I                               I S                                                             D D D S                                 
    ----
    fastspeech.v2.gl
    id: (lj050_0060)
    Scores: (#C #S #D #I) 92 0 2 3
    REF:  s u b v e r s i v e s u l t r a r i G H t i s t s r a c * i s t s a n d f a s c i s t s a * * p o s s e s s i n g e m o t i o n a l i n s t a b i l i t y o r i r r a t i o n a l b e h a v i o r 
    HYP:  s u b v e r s i v e s u l t r a r i * * t i s t s r a c E i s t s a n d f a s c i s t s a R E p o s s e s s i n g e m o t i o n a l i n s t a b i l i t y o r i r r a t i o n a l b e h a v i o r 
    Eval:                                     D D                 I                                 I I                                                                                                     

### wav

| type | wav |  
| --- | --- |  
| fastspeech v1 | <audio src="fastspeech.v1.gl/LJ050-0060.wav" controls></audio> |  
| fastspeech v2 | <audio src="fastspeech.v2.gl/LJ050-0060.wav" controls></audio> |  
