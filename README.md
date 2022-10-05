# SFDC_Opportunity_Trigger
This is a Trigger for Opportunity &amp; Opportunity Line Item.

## Trigger

<html>
  <body>
1. <br/>
Opportunity의 현재 stage와 상관없이, <br/>
stage가 negotiation으로 update 되고, <br/>
Opportunity Line Item이 존재하면, (그리고 Quote가 없다면,) <br/>
Quote를 생성한다.
<br/><br/>
2. <br/>
그리고 위에 만들어진 Quote에 Quote Line Item을 함께 추가한다.
<br/><br/>
3. <br/>
Opportunity Line Item 생성시, 업데이트시, 삭제시, <br/>
    <b>"가장 최근에 생성된"</b> Quote의 Status가 draft이면, <br/>
Quote Line Item에 <br/>
생성, 업데이트, 삭제한 Opportunity Line Item과 동일한 Product 생성, 업데이트, 삭제

  </body>
</html>
