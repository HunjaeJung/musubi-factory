# Kinesis Stream

우선 AWS 공식 문서에 나와있는 [키 컨셉](http://docs.aws.amazon.com/streams/latest/dev/key-concepts.html)을 가장 먼저 읽어보면 좋다.

![](http://docs.aws.amazon.com/ko_kr/streams/latest/dev/images/architecture.png)

위 그림에서 보는 것처럼 Kinesis Stream의 핵심 역할은 **여러 소스에서 데이터를 받아, 여러 데이터 소비자에게 전달하는 것**이다.

## Kinesis Firehose와 Kinesis Stream과 차이

AWS Kinesis 서비스에 들어가보면 총 3가지(Stream, Firehose, Analytics) 서비스가 존재한다. Analytics는 Stream과 Firehose에 들어오는 데이터들을 분석할 수 있는 서비스(SQL 사용 가능)이고, Stream과 Firehose는 데이터를 받아서 전달하는 역할을 동일하게 가지고 있다.

## SQS와 Kinesis Stream과 차이


