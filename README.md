# 송영집 (Song Yeongjip)

**시스템경영공학과 4학년 | 성균관대학교 (SKKU)**  
📧 yeongjibs@gmail.com | 🔗 [GitHub](https://github.com/zero-zip)

---

## 🎓 Education

- **성균관대학교** 시스템경영공학과 (재학 중, 2021 ~ )

---

## 🔬 Research Experience

### 스마트팩토리 캡스톤디자인1 — 1팀 (2026)
**3DGS 기반 형상-자세 공동 정제를 통한 6D 객체 자세 추정**  
*6D Object Pose Estimation via 3DGS-based Joint Shape-Pose Refinement*

> 참여기업: ㈜제이앤엘테크 | 지도교수: 정종필 교수  
> 팀원: 곽연규, 최동혁, 이승욱, 송영집

**담당 역할**: 참고 자료 수집, 보고서 작성, 관련 연구 분석

**연구 요약**  
단일 RGB-D anchor 이미지 한 장만으로 처음 보는 물체의 6D 자세(회전 R + 위치 t)를 추정하는 model-free 기법. 베이스라인 Any6D(CVPR 2025)의 근본 한계인 생성 메시의 부정확성을 극복하기 위해, 메시를 미분 가능한 3D Gaussian Splatting(3DGS)으로 변환하고 형상(shape)과 자세(pose)를 EM 교대 최적화로 공동 정제.

**3-Stage 파이프라인**
- Stage 1 — Base Estimator: 메시 생성·정렬 → 초기 자세 T(A→Q)
- Stage 2 — Mesh-to-3DGS 변환: 미분 불가 메시 → 미분 가능 3DGS (표면 점 샘플링 → 점별 가우시안 속성 부여)
- Stage 3 — Joint Shape-Pose Refinement: Shape Step(자세 고정 → 형상 gradient 역전파) ↔ Pose Step(형상 고정 → R, t 갱신) 교대 반복

**실험 결과 (HO3D, 13 sequences, 2,008 frames)**

| Metric | Any6D (Baseline) | Ours | Δ |
|--------|-----------------|------|---|
| ADD recall@0.1d | 41.0% | **45.1%** | **+4.1%p** |

---

## 📄 Research Outputs

### Program Registration (SW등록)
- **6D Object Pose Estimation via 3DGS-based Joint Shape-Pose Refinement**  
  (3DGS 기반 형상-자세 공동 정제를 통한 6D 객체 자세 추정 프로그램)  
  등록번호: C-2026-030961 | 등록일: 2026.06.23 | 저작자: 성균관대학교산학협력단

### Patent (특허출원)
- **3차원 가우시안 스플래팅 기반 형상-자세 공동 정제를 통한 6D 객체 자세 추정 방법**  
  참조번호: R-2026-0669-KR-1 | 출원인: 성균관대학교산학협력단 | 상태: 심사 중

### Conference (컨퍼런스)
- ACCV 2026 제출 예정

---

## 📚 Paper Review (팀 논문 세미나 발표)

| 발표자 | 논문 | 학회/연도 |
|--------|------|-----------|
| 곽연규 | Any6D: Model-free 6D Pose Estimation of Novel Objects | CVPR 2025 |
| **송영집** | **FoundationPose: Unified 6D Pose Estimation and Tracking of Novel Objects** | **CVPR 2024** |
| 최동혁 | GS-Pose: Generalizable Segmentation-based 6D Object Pose Estimation with 3D Gaussian Splatting | 3DV 2025 |

---

## 🛠 Skills

- **언어**: Python, MATLAB/Octave, SQL
- **분야**: Computer Vision, 6D Pose Estimation, 3D Gaussian Splatting, 최적화
- **도구**: PyTorch, Git

---

## 📬 Contact

- 이메일: yeongjibs@gmail.com
- GitHub: https://github.com/zero-zip
