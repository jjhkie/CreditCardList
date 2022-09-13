
# [ Firebase RealTime Database 를 사용한 카드 리스트 ]
 
## [ 사용한 기술 ]

  - FirebaseDatabase


## [ Point ]

  - TableView Cell 은 XIB File 을 통해 그릴 수 있다.

        [ v ] Class 생성할 때, Also create XIB file Option Check 

  - .xcworkspace 파일에 대한 정의 

  - DatabaseReference를 통해 Database 접근 

        [ v ]  var ref: DatabaseReference!
               ref = Database.database().reference() 


## [ Add ]

  - UINib

  - TableView 

    [ v ] numberOfSection __ [ 섹션의 수를 리턴하는 함수 ] 

    [ v ] numberOfRowsInSection __ [ 섹션 안에 있는 row(행)의 갯수를 리턴해주는 함수 ]
    
    [ v ] cellForRowAt __ [ UITableViewCell 하나를 리턴해주는 함수 ]
    
    [   ] estimatedHeightForRowAt
    
    [ v ] didSelectRowAt [ row에 해당하는 부분을 클릭(선택)하는 이벤트 발생 시 어떤 동작을 수행할 지를 리턴해주는 함수 ]
    


    #### Swipe Delete를 사용하기 위해 선언해줘야 하는 함수

    
     [ v ] canEditRowAt [ tableView 의 열을 편집이 가능한 지 리턴해주는 함수 ]

     [ v ] commit editingStyle: [ 스와이프했을 때 사용할 기능을 설정하는 함수 ]
