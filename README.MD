# BgLabelControl 사용하기

## 실행화면
![스크린샷 2023-12-04 105217](https://github.com/CommercialCrew/BgLabelControlApp/assets/101386134/e07f3b0f-dc38-4029-85a8-063b55b08a1e)

## 설명
"내가 직접 만든 컨트롤을 이용해" 라벨 중에서도 배경 색을 입힌 라벨을 띄우는게 목적이며, 따라서 기존의 컨트롤이 아닌 사용자 지정 컨트롤 파일을 추가해 구현한다.

실제로 MainWindows.Xaml에서 해당 컨트롤을 추가할 때, " <local:BgLabelControl ~~~" 와 같이 쓴다.

사용자 지정 컨트롤을 선택했을 때 추가되는 xaml, h, cpp 파일을 이용해 라벨부를 구현한 뒤,
Themes/Generic.xaml 파일을 통해 배경 부분을 구현한다. 여기에서 배경 부분의 크기를 얼마만큼 할지 등을 결정한다.
마지막으로 MainWindows.Xaml에 적용할 때는 위에서 이야기한 local 태그 이외에도 헤더 파일에 내가 만든 컨트롤의 헤더파일을 include 해줘야 한다.
