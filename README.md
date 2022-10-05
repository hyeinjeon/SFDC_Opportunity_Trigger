# SFDC_Opportunity_Trigger
This is a Trigger for Opportunity &amp; Opportunity Line Item.

## <Trigger>

1. 
Opportunity의 현재 stage와 상관없이,
stage가 negotiation으로 update 되고, 
Opportunity Line Item이 존재하면, (그리고 Quote가 없다면,)
Quote를 생성한다.

2. 
그리고 Quote Line Item을 함께 추가한다.

3.
Opportunity Line Item 생성시, 업데이트시, 삭제시,
가장 최근에 생성된 Quote의 Status가 draft이면, 
Quote Line Item에
생성한 Opportunity Line Item과 동일한 Product 생성, 업데이트, 삭제

