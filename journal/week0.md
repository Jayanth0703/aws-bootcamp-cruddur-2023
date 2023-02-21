# Week 0 — Billing and Architecture

Installed AWS CLI it was bit difficult in the start to syn with AWS IIAM user later it worked perfectly fine 
Have some problem with environment variables so I havent created variables.

But AWS CLI is working perfectly as expected
(> aws sts get-caller-identity
{
    "UserId": "AIDA***UHACIANCEPS***",
    "Account": "34**676**0**",
    "Arn": "arn:aws:iam::3478**644**8:user/Jayanth"
}![image](https://user-images.githubusercontent.com/60100266/220217850-b5775bfc-adce-4592-a929-60428d28a596.png)
)

Message alert enabled with topic method
    aws sns subscribe \
    --topic-arn="arn:aws:sns:eu-north-1:********:billing-alarm" \
    --protocol=email \
    --notification-endpoint=user@gmail.com
    
    Create Alarm completed

aws cloudwatch put-metric-alarm --cli-input-json file://aws/json/alarm_config.json

Create a AWS budget completed

LUCID chart created 
!.[Crudder Logical design].(Logical AWS Diagram.png)
