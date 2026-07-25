#정보관리기술사 #AI #VLM #멀티모달 #AI/LLM/생성AI #NEW
## 정의
VLM(Vision Language Model)
- Computer Vision(이미지)과 NLP(텍스트)를 결합·처리하는 멀티모달 AI 모델
## 키워드
* Multi-modal, Image Encoder, Vision-Language Projector, Shared Embedding, Cross Attention
## 암기법
* 영투디: Encoder·Projector·Decoder
## 특징
- Image Encoder(ViT·CLIP) + Language Model(Decoder)
- 융합: Cross Attention, PrefixLM, Contrastive Learning
- 도입 3대 핵심: 맥락 이해, Few-shot+Fine-tuning, 7B~10B 적정 규모
## 목적
- 이미지-텍스트 통합 이해·생성
- VQA·캡션·검색 등 멀티모달 응용
## 구성요소
- Language Encoder: BERT, RoBERTa
- Vision Encoder: ViT, CNN, CLIP
- Fusion: Cross Attention, PrefixLM, Contrastive
- Output: LLM Decoder
## 구성도
```
Image→Encoder→Projector→Shared Embedding←Tokenizer→LLM Decoder→Text
```
## 연관 토픽
- [[VLA 모델]] - Vision-Language-Action
- [[멀티모달(Multi Modal) AI]] - 멀티모달
- [[대형개념모델(LCM)]] - 개념 모델
