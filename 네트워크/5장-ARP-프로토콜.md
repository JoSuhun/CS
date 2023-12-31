# [ARP 프로토콜](https://youtu.be/LDsp-Xb168E?list=PL0d8NnikouEWcF1jJueLdjRIC4HsUlULi)

## ARP가 하는 일
- ARP프로토콜은 같은 네트워크 대역에서 통신을 하기 위해 필요한 MAC주소를 IP주소를 이용해서 알아오는 프로토콜이다.
- 같은 네트워크 대역에서 통신을 한다 하더라도, 데이터를 보내기 위해서는 7계층부터 캡슐화를 통해 데이터를 보낸다. 이 때문에, IP주소와 MAC주소가 모두 필요하다.
- 이때 IP주소는 알고 MAC주소는 모르더라도, ARP를 통해 통신이 가능하다.

### ARP 구조
- IP주소를 이용해 MAC주소를 알아오는 ARP 프로토콜

## ARP 프로토콜의 통신 과정
- 하나의 네트워크 대역일 때
![image1](./5%EC%9E%A5/arp.png)
    1.  보내는 컴퓨터에서는 ARP 요청
    2. 이더넷 프로토콜 encapsulation 하여 보냄
    3. 출발지의 MAC주소와 IP주소에 각각 자신의 주소를 써서 다시 보내줌
    4. ARP 캐시 테이블에 내용 등록

### ARP 테이블
- 통신 했던 컴퓨터들의 주소는 ARP 테이블에 남는다.
