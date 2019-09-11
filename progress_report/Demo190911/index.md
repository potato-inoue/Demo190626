# demo190911

## speaker 1089  

### Training condition & attention_weight

| ID | **0th decode** | **rev1** |  
| --- | --- | --- |  
| lr | 1e-4 | 1e-4 |  
| atype |  location | location |  
| use-guided-attn-loss | <span style="color: red; ">true</span> | <span style="color: red; ">true</span> |  
| guided-attn-loss-sigma | 0.4 | 0.4 | - | - |  
| reduction-factor | <span style="color: red; ">2</span> | <span style="color: blue; ">3</span> | <span style="color: blue; ">3</span> | <span style="color: red; ">2</span> |  
| batch-size | 16 | 16 | 16 | 16 |  
| Max_epoch | 100 | 100 | 100 | 100 |  
| Patience | 0 | 0 | 0 | 0 | 
| Best_epoch | - | - | - | - |  
| End_epoch | 100 | 100 | 100 | 100 |  
| 1st epoch | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev1/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.1.png" width="320px"> | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev2/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.1.png" width="320px"> | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev3/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.1.png" width="320px"> | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev4/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.1.png" width="320px"> |  
| 2nd epoch | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev1/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.2.png" width="320px"> | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev2/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.2.png" width="320px"> | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev3/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.2.png" width="320px"> | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev4/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.2.png" width="320px"> |  
| 3rd epoch | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev1/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.3.png" width="320px"> | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev2/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.3.png" width="320px"> | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev3/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.3.png" width="320px"> | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev4/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.3.png" width="320px"> |  
| 4th epoch | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev1/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.4.png" width="320px"> | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev2/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.4.png" width="320px"> | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev3/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.4.png" width="320px"> | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev4/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.4.png" width="320px"> |  
| 5th epoch | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev1/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.5.png" width="320px"> | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev2/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.5.png" width="320px"> | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev3/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.5.png" width="320px"> | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev4/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.5.png" width="320px"> |  
| ... | ... | ... | ... | ... |  
| 100th epoch | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev1/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.100.png" width="320px"> | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev2/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.100.png" width="320px"> | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev3/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.100.png" width="320px"> | <img src="blizzard17/train_no_dev_pytorch_train_pytorch_tacotron2.tuning.lab3-rev4/results/att_ws/TheMusiciansOfBremen_21_Track_21_000185-000429.ep.100.png" width="320px"> |   

### 1089_134691_000043_000000  
[1]

| ground_truth | **0th decode** | **rev1** |  
| --- | --- | --- |  
| <audio src="libritts_asrtts_offline/ground_truth/eval/wav/1089_134691_000043_000000.wav" controls></audio> | <audio src="libritts_asrtts_offline/sample_rev2_train_pytorch_tts_train_pytorch_transformer.fine-tuning.rev0/eval/wav/1089_134691_000043_000000.wav" controls></audio> <br> <img src="libritts_asrtts_offline/sample_rev2_train_pytorch_tts_train_pytorch_transformer.fine-tuning.rev0/eval/wav/1089_134691_000043_000000_att_ws.png" width="320px"> | <audio src="libritts_asrtts_offline/sample_rev2_train_pytorch_tts_train_pytorch_transformer.fine-tuning.rev1/eval/wav/1089_134691_000043_000000.wav" controls></audio> <br> <img src="libritts_asrtts_offline/sample_rev2_train_pytorch_tts_train_pytorch_transformer.fine-tuning.rev1/eval/wav/1089_134691_000043_000000_att_ws.png" width="320px"> |   

### 1089_134691_000044_000001  
"He was unheeded, happy and near to the wild heart of life."  

| ground_truth | **0th decode** | **rev1** |  
| --- | --- | --- |  
| <audio src="libritts_asrtts_offline/ground_truth/eval/wav/1089_134691_000044_000001.wav" controls></audio> | <audio src="libritts_asrtts_offline/sample_rev2_train_pytorch_tts_train_pytorch_transformer.fine-tuning.rev0/eval/wav/1089_134691_000044_000001.wav" controls></audio> <br> <img src="libritts_asrtts_offline/sample_rev2_train_pytorch_tts_train_pytorch_transformer.fine-tuning.rev0/eval/wav/1089_134691_000044_000001_att_ws.png" width="320px"> | <audio src="libritts_asrtts_offline/sample_rev2_train_pytorch_tts_train_pytorch_transformer.fine-tuning.rev1/eval/wav/1089_134691_000044_000001.wav" controls></audio> <br> <img src="libritts_asrtts_offline/sample_rev2_train_pytorch_tts_train_pytorch_transformer.fine-tuning.rev1/eval/wav/1089_134691_000044_000001_att_ws.png" width="320px"> |   

### 1089_134691_000045_000003  
"Her thighs, fuller and soft hued as ivory, were bared almost to the hips, where the white fringes of her drawers were like feathering of soft white down."  

| ground_truth | **0th decode** | **rev1** |  
| --- | --- | --- |  
| <audio src="libritts_asrtts_offline/ground_truth/eval/wav/1089_134691_000045_000003.wav" controls></audio> | <audio src="libritts_asrtts_offline/sample_rev2_train_pytorch_tts_train_pytorch_transformer.fine-tuning.rev0/eval/wav/1089_134691_000045_000003.wav" controls></audio> <br> <img src="libritts_asrtts_offline/sample_rev2_train_pytorch_tts_train_pytorch_transformer.fine-tuning.rev0/eval/wav/1089_134691_000045_000003_att_ws.png" width="320px"> | <audio src="libritts_asrtts_offline/sample_rev2_train_pytorch_tts_train_pytorch_transformer.fine-tuning.rev1/eval/wav/1089_134691_000045_000003.wav" controls></audio> <br> <img src="libritts_asrtts_offline/sample_rev2_train_pytorch_tts_train_pytorch_transformer.fine-tuning.rev1/eval/wav/1089_134691_000045_000003_att_ws.png" width="320px"> |   

### 1089_134691_000045_000004  
"Her slate blue skirts were kilted boldly about her waist and dovetailed behind her."  

| ground_truth | **0th decode** | **rev1** |  
| --- | --- | --- |  
| <audio src="libritts_asrtts_offline/ground_truth/eval/wav/1089_134691_000045_000004.wav" controls></audio> | <audio src="libritts_asrtts_offline/sample_rev2_train_pytorch_tts_train_pytorch_transformer.fine-tuning.rev0/eval/wav/1089_134691_000045_000004.wav" controls></audio> <br> <img src="libritts_asrtts_offline/sample_rev2_train_pytorch_tts_train_pytorch_transformer.fine-tuning.rev0/eval/wav/1089_134691_000045_000004_att_ws.png" width="320px"> | <audio src="libritts_asrtts_offline/sample_rev2_train_pytorch_tts_train_pytorch_transformer.fine-tuning.rev1/eval/wav/1089_134691_000045_000004.wav" controls></audio> <br> <img src="libritts_asrtts_offline/sample_rev2_train_pytorch_tts_train_pytorch_transformer.fine-tuning.rev1/eval/wav/1089_134691_000045_000004_att_ws.png" width="320px"> |   

### 1089_134691_000045_000005  
"Her bosom was as a bird's, soft and slight, slight and soft as the breast of some dark plumaged dove."   

| ground_truth | **0th decode** | **rev1** |  
| --- | --- | --- |  
| <audio src="libritts_asrtts_offline/ground_truth/eval/wav/1089_134691_000045_000005.wav" controls></audio> | <audio src="libritts_asrtts_offline/sample_rev2_train_pytorch_tts_train_pytorch_transformer.fine-tuning.rev0/eval/wav/1089_134691_000045_000005.wav" controls></audio> <br> <img src="libritts_asrtts_offline/sample_rev2_train_pytorch_tts_train_pytorch_transformer.fine-tuning.rev0/eval/wav/1089_134691_000045_000005_att_ws.png" width="320px"> | <audio src="libritts_asrtts_offline/sample_rev2_train_pytorch_tts_train_pytorch_transformer.fine-tuning.rev1/eval/wav/1089_134691_000045_000005.wav" controls></audio> <br> <img src="libritts_asrtts_offline/sample_rev2_train_pytorch_tts_train_pytorch_transformer.fine-tuning.rev1/eval/wav/1089_134691_000045_000005_att_ws.png" width="320px"> |   

[1] "Where was his boyhood now?" 
