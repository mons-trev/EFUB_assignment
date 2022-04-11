# EFUB_assignment

# EFUB 4주차 세미나 과제

###### 프백 인턴 변지은



### 01. 학사 정보 관리 ERD


![다이어그램](https://user-images.githubusercontent.com/80975932/162748677-a0146493-c077-492a-bbd5-a20adb3c020d.PNG)



### 02. MySQL 실습 코드

##### SWS 테이블 생성 코드

```
CREATE TABLE sws (
team_id int not null,
name varchar(10) not null,
PRIMARY KEY(team_id)
);
```



##### JOIN 코드

```
select member.name, position, email, birth_date, swsteam, sws.name
from member, sws
where member.swsteam = sws.team_id;
```



##### JOIN 출력 결과


![join](https://user-images.githubusercontent.com/80975932/162748927-a691daf1-8ddc-4e3d-891d-54b353551e5e.PNG)
