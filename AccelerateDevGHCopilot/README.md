# Library App

## Description
Library App은 .NET 기반의 라이브러리 관리 시스템 예제 프로젝트입니다. 이 프로젝트는 도메인 계층, 인프라 계층, 콘솔 애플리케이션, 그리고 단위 테스트로 구성되어 있으며, 확장성과 유지보수성을 고려한 구조를 갖추고 있습니다.

## Project Structure
- AccelerateDevGHCopilot/
  - AccelerateDevGHCopilot.sln
  - src/
    - Library.ApplicationCore/
      - Library.ApplicationCore.csproj
      - Entities/
      - Enums/
      - Interfaces/
      - Services/
    - Library.Console/
      - appSettings.json
      - CommonActions.cs
      - ConsoleApp.cs
      - ConsoleState.cs
      - Library.Console.csproj
      - Program.cs
      - README.md
      - Json/
    - Library.Infrastructure/
      - ...
  - tests/
    - UnitTests/
      - ...

## Key Classes and Interfaces
- `Entities/`
  - 도메인 엔티티 클래스들이 위치합니다. 예: Book, User 등
- `Enums/`
  - 도메인에서 사용하는 열거형 타입 정의
- `Interfaces/`
  - 서비스 및 저장소 인터페이스 정의
- `Services/`
  - 비즈니스 로직을 구현한 서비스 클래스
- `Library.Console/ConsoleApp.cs`
  - 콘솔 애플리케이션의 진입점 및 주요 실행 로직
- `Library.Console/CommonActions.cs`
  - 콘솔에서 공통적으로 사용하는 액션 및 유틸리티 함수

## Usage
1. 저장소를 클론합니다.
   ```sh
   git clone <repository-url>
   ```
2. 필요한 .NET SDK가 설치되어 있는지 확인합니다.
   ```sh
   dotnet --version
   ```
3. 솔루션을 복원하고 빌드합니다.
   ```sh
   dotnet restore
   dotnet build
   ```
4. 콘솔 애플리케이션을 실행합니다.
   ```sh
   dotnet run --project AccelerateDevGHCopilot/src/Library.Console/Library.Console.csproj
   ```
5. 단위 테스트를 실행합니다.
   ```sh
   dotnet test
   ```

## License
이 프로젝트는 MIT 라이선스 하에 배포됩니다.