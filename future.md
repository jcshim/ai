Hailo-8은 엣지에서 고속 얼굴인식 처리하는 NPU라서, 보안·매장 분석 같은 얼굴인식 비즈니스에 딱 맞아. 각 AI 단계별로 Hailo-8 얼굴인식 시스템에 적용한 비즈니스 예시를 간단히 정리할게. [fishpoint.tistory](https://fishpoint.tistory.com/11382)

## LLM/기본 AI
**매장 입장 고객 카운팅**  
Hailo-8 카메라가 얼굴 감지하면 LLM이 "오늘 50명 입장" 텍스트 리포트 생성. 단순 출력만 하고 끝. [fishpoint.tistory](https://fishpoint.tistory.com/11382)

## AI 에이전트
**VIP 고객 자동 환영**  
얼굴인식 → 고객 DB 조회 → "김○○님 오셨습니다" 음성 출력 + 포인트 적립 API 호출. 하나의 에이전트가 인식부터 액션까지 자율 처리. [hailo](https://hailo.ai/ja/blog/multi-camera-multi-person-re-identification/)

## 멀티 에이전트
**실시간 재고 보충 시스템**  
- **인식 에이전트**: Hailo-8로 얼굴 감지 (누가 왔는지)  
- **분석 에이전트**: 구매 패턴 분석 (무엇을 자주 사는지)  
- **실행 에이전트**: 재고 부족 시 자동 발주 API 호출  
3개 에이전트가 협업해 완전 자동화. [fishpoint.tistory](https://fishpoint.tistory.com/11382)

## Agentic AI
**완전 자율 매장 운영**  
"매출 20% 증가시키자" 목표 주면:  
1. Hailo-8 얼굴 데이터로 고객층 분석  
2. 할인 쿠폰 자동 생성·발송  
3. 다음날 재고 자동 조정  
4. 효과 측정 후 전략 수정  
인간 지시 없이 목표만 주면 스스로 최적화. [hailo](https://hailo.ai/ja/blog/multi-camera-multi-person-re-identification/)

## 비즈니스 가치 비교
| 단계 | Hailo-8 역할 | 매출 영향 |
|------|-------------|----------|
| LLM | 얼굴→텍스트 | 기본 리포트 |
| 에이전트 | 인식+액션 | 15% 효율↑ |
| 멀티 | 팀 협업 | 35% 자동화 |
| Agentic | 완전 자율 | 60%+ 매출↑ |

임베디드 연구자라면 Hailo-8 + Pico W 조합으로 **에이전트** 단계부터 실험 시작 추천. YOLO 얼굴인식 모델 컴파일해서 TAPPAS 파이프라인 돌려봐. [fishpoint.tistory](https://fishpoint.tistory.com/11382)
