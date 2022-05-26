<img width="453" alt="Capture" src="https://user-images.githubusercontent.com/105406807/170453014-9d6df54c-77da-4432-b88c-9bc2ef74d330.PNG">




```sql
create table Match (
MId INTEGER,
TId INTEGER references tournament(tid),
Player1 INTEGER  references player(pid),
Player2 INTEGER  references player(pid),
MatchDt DATE NOT NULL,
Winner	 INTEGER references player(pid),
Score  VARCHAR2(30)	NOT NULL,
constraint pk primary key(MId,TId),
constraint ck check (Player1<>Player2));
```
