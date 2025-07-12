# CCE


주차	    학습·훈련 포커스	          실전 시뮬레이션	            목표 체크포인트

W1 (D‑28 ~ D‑22)	기초 다지기	환경 세팅: Ubuntu + pwndbg, Ghidra, radare2, Python 3.12, Burp Suite Community, Volatility3, CyberChef. Baseline 테스트: pwn.college Module 9 “Binary Exploitation” 5문제, PortSwigger Mystery Lab 3문제. 역공 노트: 개인 위키·Obsidian에 카테고리별 치트시트 작성 시작.	하루 30‑min “스피드 런”(write‑up 보고 그대로 재현) 1 회.	▸ 환경 완비 ▸ 치트시트 v0.1 완성


W2 (D‑21 ~ D‑15)	포너블 집중	ROP Emporium Ret2win→Split→Callme→Ropchain 전부 풀이. pwn.college Module 10 ECB‑to‑Shellcode easy/hard. 리버싱: Crackmes.one 3‑5점 난이도 3개.	토·일에 6 h 미니‑CTF(CTFtime Archive에서 2024 년 3‑4시간 분량 대회 재현).	▸ ROP 스택 pivot까지 자력 솔브 ▸ gdb + gef/pwndbg 매크로 정리


W3 (D‑14 ~ D‑8)	멀티 카테고리	웹: PortSwigger all‑labs에서 CSRF, SSTI, Prototype Pollution 각 3개. 암호: CryptoHack General·RSA·Diffie‑Hellman 20문제. 포렌식: Volatility3 Linux 튜토리얼 따라하며 메모리 이미지 2개 분석. 수요일: 팀원과 4 h 모의 CCE(분야별 3‑3‑2‑2‑2 문제 구성).	▸ 평균 풀이 속도 30 min/200점 문제 목표


W4 (D‑7 ~ D‑1)	실전 최적화	모의 예선(9 h 풀타임) 금요일 실시 → 점수·타임라인 기록. 남은 기간 = 오답 복기 + 치트시트 v1.0 확정판.	• 인프라 리허설: 동일 네트워크, 한글·영문 키보드 단축키 체크. • 멘탈·체력 관리: 수면 리듬 대회 시간대에 맞춤.	▸ 모의전 점수 ≥ 작년 예선 합격컷 120% 목표



첫번째 도전과제

cd ~/pwn || mkdir ~/pwn && cd ~/pwn

wget https://ropemporium.com/binary/ret2win

chmod +x ret2win

gdb ./ret2win

이걸 붙여넣기 하고

https://ropemporium.com/ 여기 들어가서 ret2win문제풀이. 풀면 다른문제도. 만약 너무 처음이라 헷갈린다 -- 그냥 구글에서 ret2win writeup이라고 친 다음에 답 확인하고 왜 그런지만 학습하면 됨.
2~3문제 하고 나면 약간 감 잡힐수도?
