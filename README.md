
[ Firebase RealTime Database 를 사용한 카드 리스트 ]

[ 사용하 기술 ]

- FirebaseDatabase


[ Point ]

- TableView Cell 은 XIB File 을 통해 그릴 수 있다.
  > Class 생성할 때, Also create XIB file Option Check 

- .xcworkspace 파일에 대한 정의 

- DatabaseReference를 통해 Database 접근 


[ Add ]

- UINib

- TableView 
  > numberOfRowsInSection
  > cellForRowAt
  > estimatedHeightForRowAt
  > didSelectRowAt
  > canEditRowAt
  > commit editingStyle:
