# **Aero Simulator**

![22222](https://github.com/user-attachments/assets/d5aa9356-81d2-4ea7-9775-08a552f03b15)

## **프로젝트 소개**
Aero Simulator는 브라우저 기반의 실시간 2D 유체 시뮬레이터로, 사용자가 유체의 흐름을 시각화하고, 물체와의 상호작용에 따른 항공역학적 데이터를 분석할 수 있는 도구입니다.  
Euler 방법과 Semi-Lagrangian 방식을 활용하여 다양한 유체 시뮬레이션 환경을 제공합니다.

## **기능**
- **실시간 유체 시뮬레이션**:
  - Wind Tunnel(풍동) 환경 시뮬레이션.
  - Streamline(유선) 및 Pressure(압력) 시각화.
- **사용자 조작**:
  - 장애물의 위치 및 크기를 드래그로 실시간 변경.
  - 중력, 압축성, Advection(운반) 등 매개변수 조정 가능.
- **항공역학 계산**:
  - 양력(Lift) 및 항력(Drag) 값을 실시간 계산 및 표시.

## **주요 기술**
### **1. 유체 시뮬레이션 방식**
- **Euler 방법**: 격자(Grid) 기반으로 고정된 위치에서 유체의 속성을 계산.
- **Semi-Lagrangian 방법**: 유체 입자의 이전 위치를 추적하여 값을 업데이트.

### **2. 물리적 계산**
- **중력 효과 적용**: `integrate(dt, gravity)`
- **압축성 유지**: `solveIncompressibility(numIters, dt)`
- **운반 과정 시뮬레이션**: `advectSmoke(dt)`, `advectVel(dt)`

### **3. 시각화**
- 연기(Smoke) 밀도 및 압력(Pressure) 필드 표현.
- Streamline(유선) 계산 및 렌더링.

## **구현 상세**
### **기술 스택**
- **HTML5 Canvas**: 유체 흐름의 그래픽 표현.
- **JavaScript**: 물리 엔진 및 시뮬레이션 로직 구현.
- **CSS**: UI 디자인 및 스타일링.

## **설치 및 실행**
### **1. 클론**
```bash
git clone https://github.com/yourusername/aero-simulator.git
cd aero-simulator
```

### **2. 로컬 실행**
웹 브라우저에서 `index.html` 파일을 열어 실행합니다.

### **3. GitHub Pages 배포**
GitHub Pages를 통해 프로젝트를 배포할 수 있습니다:
1. `Settings > Pages`로 이동.
2. 배포 브랜치 선택 후 URL을 확인.

## **결과 및 시뮬레이션 예시**
### **1. Wind Tunnel**
![11111](https://github.com/user-attachments/assets/75660c51-1564-44f5-b260-e95e4bc7b473)
유체가 풍동 환경에서 장애물을 통과하며 흐르는 모습을 시각화합니다.

### **2. Streamline**
![22222](https://github.com/user-attachments/assets/220ed9bb-0b56-45b5-8d2a-6d4dca85edca)
유선 표현을 통해 유체의 흐름 방향과 속도를 시각화합니다.

### **3. Pressure**
![33](https://github.com/user-attachments/assets/3a06cb12-d39a-43cc-b803-f0cc5d9a0988)
압력 필드를 계산하고, 색상으로 시각화합니다.

## **한계점 및 향후 과제**
1. **3D 확장**:
   - 2D 격자를 3D로 확장하여 입체적인 유체 흐름 표현.
2. **유체 점성 추가**:
   - 내부 마찰력을 반영하여 현실적인 흐름 구현.
3. **다양한 장애물 처리**:
   - 복잡한 동적 경계 조건 및 객체 추가 가능성.

## **기여 방법**
1. 이 프로젝트를 포크합니다.
2. 새로운 브랜치를 생성합니다: `git checkout -b feature-name`
3. 변경 사항을 커밋합니다: `git commit -m "Add feature"`
4. 브랜치에 푸시합니다: `git push origin feature-name`
5. Pull Request를 생성합니다.

## **팀**
- **202128683 이지수**  
- **202128682 최윤재**
