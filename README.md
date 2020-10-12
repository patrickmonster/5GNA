5G vRAN 지원 에너지 효율적인 비디오 스트리밍 시스템

5G vRAN-assisted Energy Efficient Video Streaming System

1.1 연구 배경

  4세대 이동통신에서 5세대 이통 통신으로 변경되면서 Client들이 5G에 관한 관심과 연구가 가속화도고 있다. 5G통신을 이용한 스마트 팩토리, 자율주행등 많은 연구가 이루어지고 있다. 이에 따른 VR 미디어 시대가 시작되면서, VR을 이용한 미디어가 활발히 제작되고 있다. 이러한 컨텐츠를 다운받는 시스템은 구축이 되어 있으나, 컨텐츠를 실시간으로 보던 도중에 꺼버리는 경우나 혹은 장거리 통신을 할 때에 중간에 거치는 Server가 없기 때문에 버퍼링이 생기는 경우도 있다. 본 논문은 이러한 문제점들을 개선하고 클아이언트 측에서 모든 정보를 저장하는 대신, vRan 클라우드에 일부 저장하여 원활한 통신을 하며 동시에 무선 통신망의 데이터를 감소시키는 것을 목표로 하고 있다.
  
1.2 연구 목적

대부분의 VR 어플들은 콘텐츠 자체를 불러올 때에 일정이상의 미디어 데이터를 수신 받거나 재생 중간에도 최소 크기의 버퍼가 불러와져야 재생이 된다. 특히나 모바일 Client는 PCClient보다 더 자주 동영상 재생을 그만두는 경향이 있어[1], 이로 인하여 버퍼에 사용되지 않은 비디오 데이터가 낭비 될 수 있다. 이러한 문재를 해결하기 위하여 5G 시스템의 vRan을 사용하여 버퍼 리소스를 효율적으로 사용하여 모바일 장치의 에너지 소비를 줄이면서 안정적인 비디오 스트리밍 서비스를 Client에게 제공하는 것을 구현한다.

1.3 연구 내용 및 범위

본 연구는 Linux Ubuntu 20.04 를 이용하여 실험하였고, 실험 프로그램으로써는 Node.js와 Python 을 이용하여 Server 및 Client를 구축하였다. 또한 라즈베리 파이를 이용하여 무선 통신 환경을 구축하여 데이터를 추출하였다.


결론
 본 논문은  Split-TCP 와 MPEG DASH SRD 시스템을 이용하여 Client가 원하는 만큼 데이터를 불러오고, 이를 vRan 클라우드에 저장하여 진행하였으며 실제 네트워크 환경을 구축하여 실험하였고 실제 장거리 네트워크를 구현하기 위하여 iproute2 소프트웨어를 사용하여 Server와 Client의 연결간 부하를 주어 vRan을 통한 스트리밍을 실시하였다. 실험을 통하여 MPEG-DASH 시스템을 이용하여 고화질부터 저화질 변환을 통한 Server와 vRan 간의 네트워크 상태에 따라 화질이 변화할 수 있도록 지속적인 연구 개발을 수행할 예정이다.
