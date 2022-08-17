# LSTM-Seq2Seq-with-Attention

### Objectives
- 영한 번역기 개발을 위해 LSTM Encoder-Decoder with Attention 모델을 훈련하고 BLUE 스코어를 측정한다.

### Models and Data
- LSTM Encoder-Decoder with Attention
- AIHub 한국어-영어 번역(병렬) 말뭉치 구어체 20만건

### Envs and Requirements
- Colab
- Tensorflow, Pandas, RE

### Progress
- 성능 향상을 위한 모델 수정
- 데이터 확보 및 정제
- 토큰화 및 코퍼스 사전 구축 / 훈련 및 추론
- 추가 데이터 확보 / 시퀀스 역순 입력 / 훈련 및 추론
- BLUE 스코어 기록 경쟁

### Result
- BLUE 스코어 기록 경쟁 1위

### Retrospective
- RNN 계열 수업 후 Encoder-Decoder 모델의 원리를 익히고 Attention 기작의 효과를 확인하기 위해 진행한 프로젝트
- Attention이 포함되지 않은 LSTM Seq2Seq 모델의 레이어 구성과 하이퍼 파라미터 수정을 수차례 진행했으나 번역이라고 느껴질 만한 결과물을 만들어내지 못 함
- 동일한 데이터로 Attention을 포함한 모델이 월등히 우수한 결과물을 만들어내는 것을 확인
- Encoder-Decoder 모델에서 시퀀스 역순 입력으로 성능 향상이 가능하다는 정보를 입수해 직접 비교 실험을 실시했으나 당시 BLUE 스코어 이해 부족으로 정성 평가만 진행
- 추가 데이터로 최종 훈련을 진행하고 기록 경쟁에서 1위를 차지
- 함수형 모델 작성과 수정에 있어서 어려움이 많았기 때문에 추후 복습과 재학습의 필요성을 느낌

### References
- https://www.tensorflow.org/
- https://keras.io/
