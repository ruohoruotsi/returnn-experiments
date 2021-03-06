These are configs for encoder-decoder-attention models.

* The best baseline (without LM) is `base3.retrain2`, epoch 166,
  with 12.93% WER on dev-other.
  This is a continued training from the best model of `base3.retrain`
  (13.07% WER on dev-other, epoch 132),
  which itself is a continued training from the best model of `base2.bs18k.curric3`
  (13.32% WER, epoch 250).

* `base2.bs18k.curric3` is based on `base2.bs18k` with the modified curriculum learning,
  with 13.32% WER on dev-other in epoch 250.

* `base2.bs18k` is based on `base2` with batch size 18000 instead of 20000.

* `base2` is basically the same as `base.red6.pretrain-start2l-red6-below-grow3`.

* `base.red6.pretrain-start2l-red6-below-grow3` is the best LibriSpeech result as reported
  in the [A comprehensive analysis on attention models](https://www-i6.informatik.rwth-aachen.de/publications/download/1091/Zeyer-NIPS%20IRASL-2018.pdf) paper,
  with 13.95% WER on dev-other in epoch 239.
