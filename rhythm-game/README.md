# rhythm-game-prototype
rhythm game prototype for our SSANG

# rhythm-game-2
싱글톤 패턴 기반 구축

## GameManager

Note Json 불러오기

## NoteManager

각 라인 별로 노트를 생성, 위치 시킨다.

noteInterval : 노트 간의 간격, 보통 노트의 속도와 동일하게 맞춰주는 것이 이론적으로 맞다.

goNote : 보통 노트, 파란색

startLongNote : 롱 노트 시작, 노란색

endLongNote : 롱노트 끝, 빨간색

Line3의 경우 sec = 0인 곳에 노트를 하나 더 생성

이 노트는 보이지 않게 한다.

## StartMusic

Line3에 보면 StartFrame이 있는데

이 프레임이 시작노트를 인식하고 노래를 재생하여 싱크를 맞춘다.

## etc

json을 읽어들이지 못하는 문제 해결

GameManager에서 Start이 아닌 Awake에서 json을 불러와야 함

게임이 시작될 때 노래가 자동으로 시작되는 것이 아니라 시작노트가 지나가면 음악이 재생

Line3에서 안보이는 시작 노트가 지나가면 그때 실행된다. 
