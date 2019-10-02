# Speaker adaptation for single speaker tts model

model: ljspeech.transformer.v1
text: ASR output
speech: speech of target speaker

## 2300(M)

| rev | 1 | 2 |  
| --- | --- | --- |  
| lr | 1e0 | 1e-1 |  
| epoch | - | 100 |  
| all_loss      | <img src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1.rev1/results/all_loss.png" width="320px">           | <img src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1e-1.rev2/results/all_loss.png" width="320px">            |  
| loss          | <img src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1.rev1/results/loss.png" width="320px">               | <img src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1e-1.rev2/results/loss.png" width="320px">                |  
| l1_loss       | <img src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1.rev1/results/l1_loss.png" width="320px">            | <img src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1e-1.rev2/results/l1_loss.png" width="320px">             |  
| l2_loss       | <img src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1.rev1/results/l2_loss.png" width="320px">            | <img src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1e-1.rev2/results/l2_loss.png" width="320px">             |  
| bce_loss      | <img src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1.rev1/results/bce_loss.png" width="320px">           | <img src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1e-1.rev2/results/bce_loss.png" width="320px">            |  
| encoder_alpha | <img src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1.rev1/results/encoder_alpha.png" width="320px">      | <img src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1e-1.rev2/results/encoder_alpha.png" width="320px">       |  
| decoder_alpha | <img src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1.rev1/results/decoder_alpha.png" width="320px">      | <img src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1e-1.rev2/results/decoder_alpha.png" width="320px">       |  
| attn_loss     | <img src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1.rev1/results/enc_dec_attn_loss.png" width="320px">  | <img src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1e-1.rev2/results/enc_dec_attn_loss.png" width="320px">   |  

### target for pre-train  
<audio src="../ljspeech_asrtts_offline/ljspeech.ground_truth/eval/wav/LJ050-0029.wav" controls></audio>  

### 2300_134691_000049_000001.wav  

    Ground truth:  
    Recog output:  

| type | wav |  
| --- | --- |  
| target for fine-tuning            | <audio src="../ljspeech_asrtts_offline/test_clean_22050_2300.ground_truth/eval/wav/2300_134691_000049_000001.wav" controls></audio> |  
| 0th decode                        | <audio src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1.rev1/eval_0th/wav/2300_134691_000049_000001.wav" controls></audio> | 
| avg.best  (lr:1e0, - epoch)      | <audio src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1.rev1/eval_avg.best/wav/2300_134691_000049_000001.wav" controls></audio> |  
| avg.best  (lr:1e-1, 100 epoch)    | <audio src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1e-1.rev2/eval_avg.best/wav/2300_134691_000049_000001.wav" controls></audio> |  

### 2300_134691_000049_000002.wav  

    Ground truth:  
    Recog output:  

| type | wav |  
| --- | --- |  
| target for fine-tuning            | <audio src="../ljspeech_asrtts_offline/test_clean_22050_2300.ground_truth/eval/wav/2300_134691_000049_000002.wav" controls></audio> |  
| 0th decode                        | <audio src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1.rev1/eval_0th/wav/2300_134691_000049_000002.wav" controls></audio> |  
| avg.best  (lr:1e0, - epoch)      | <audio src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1.rev1/eval_avg.best/wav/2300_134691_000049_000002.wav" controls></audio> |  
| avg.best  (lr:1e-1, 100 epoch)    | <audio src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1e-1.rev2/eval_avg.best/wav/2300_134691_000049_000002.wav" controls></audio> |  

### 2300_134691_000049_000003.wav  

    Ground truth:  
    Recog output:  

| type | wav |  
| --- | --- |  
| target for fine-tuning            | <audio src="../ljspeech_asrtts_offline/test_clean_22050_2300.ground_truth/eval/wav/2300_134691_000049_000003.wav" controls></audio> |  
| 0th decode                        | <audio src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1.rev1/eval_0th/wav/2300_134691_000049_000003.wav" controls></audio> |  
| avg.best  (lr:1e0, - epoch)      | <audio src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1.rev1/eval_avg.best/wav/2300_134691_000049_000003.wav" controls></audio> |  
| avg.best  (lr:1e-1, 100 epoch)    | <audio src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1e-1.rev2/eval_avg.best/wav/2300_134691_000049_000003.wav" controls></audio> |  

### 2300_134691_000050_000002.wav  

    Ground truth:  
    Recog output:  

| type | wav |  
| --- | --- |  
| target for fine-tuning            | <audio src="../ljspeech_asrtts_offline/test_clean_22050_2300.ground_truth/eval/wav/2300_134691_000050_000002.wav" controls></audio> |  
| 0th decode                        | <audio src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1.rev1/eval_0th/wav/2300_134691_000050_000002.wav" controls></audio> |  
| avg.best  (lr:1e0, - epoch)      | <audio src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1.rev1/eval_avg.best/wav/2300_134691_000050_000002.wav" controls></audio> |  
| avg.best  (lr:1e-1, 100 epoch)    | <audio src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1e-1.rev2/eval_avg.best/wav/2300_134691_000050_000002.wav" controls></audio> |  

### 2300_134691_000052_000000.wav  

    Ground truth:  
    Recog output:  

| type | wav |  
| --- | --- |  
| target for fine-tuning            | <audio src="../ljspeech_asrtts_offline/test_clean_22050_2300.ground_truth/eval/wav/2300_134691_000052_000000.wav" controls></audio> |  
| 0th decode                        | <audio src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1.rev1/eval_0th/wav/2300_134691_000052_000000.wav" controls></audio> |  
| avg.best  (lr:1e0, - epoch)      | <audio src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1.rev1/eval_avg.best/wav/2300_134691_000052_000000.wav" controls></audio> |  
| avg.best  (lr:1e-1, 100 epoch)    | <audio src="../ljspeech_asrtts_offline/test_clean_22050_2300_train_no_dev_pytorch_tts_train_pytorch_transformer.fine-tuning.spk2300_lr1e-1.rev2/eval_avg.best/wav/2300_134691_000052_000000.wav" controls></audio> |  
