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
<img width="602" alt="Capture" src="https://user-images.githubusercontent.com/105406807/170476794-fc7809f0-3634-4c84-90fe-7a48a55f0f81.PNG">

```sql
create table Bill (
BillNo NUMBER primary key,
StoreName 	VARCHAR2(20) references Store(StoreName),
ShopperId NUMBER references Shopper (ShopperId),
ArCode 	CHAR(5) references Article(ArCode),
Amount NUMBER,
BillDate DATE,
Quantity NUMBER(4) default 1 constraint gg  check(Quantity>0));

```
<img width="694" alt="Capture" src="https://user-images.githubusercontent.com/105406807/170537167-359910f0-16f8-42c9-a3b1-dd12c43e94e4.PNG">
```sql
select EmpId,EmpName,Salary,
case Designation 
when 'Administrator' then Salary*1.1
when 'Billing Staff' then Salary*1.2
when 'Manager' then Salary*1.05
when 'Security' then Salary*1.25
else Salary*1.02
end 	INCREASEDSALARY
from Empdetails

```
