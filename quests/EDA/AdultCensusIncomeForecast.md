| Column         | Data Type | 설명           | 분석가 의견                                         |
| -------------- | --------- | -------------- | --------------------------------------------------- |
| id             | int64     | 고유식별자     |                                                     |
| age            | int64     | 나이           | max bound 이상은 max bound 처리 가능                |
| workclass      | object    | 직업분류       | 8가지 정도의 직업군 분류                            |
| fnlwgt         | int64     | 가중치값       | 현재 표본에서 전체 인구를 추정할 때 사용하는 가중치 |
| education      | object    | 교육 수준      | education_num과 같은 값                             |
| education_num  | int64     | 교육 수준      | education과 같은 값                                 |
| marital_status | object    | 결혼 상태      | 7가지 결혼 상태                                     |
| occupation     | object    | 직업           | 14가지 직업군                                       |
| relationship   | object    | 가족 관계      | 6가지 관계 값                                       |
| race           | object    | 인종           | 5가지 인종 값                                       |
| gender         | object    | 성별           | 두가지 성별 값                                      |
| capital_gain   | int64     | 자본 이득      | 0인 값에 대한 쏠림 심함                             |
| capital_loss   | int64     | 자본 손실      | 0인 값에 대한 쏠림 심함                             |
| hours_per_week | int64     | 주당 근무 시간 | 주당 근무 시간 분포 알수 있다                       |
| native_country | object    | 출신 국가      | 41개 국가 미국 출신이 많음                          |
| income         | object    | 소득 수준      | <=50K 또는 >50K 의 두가지 값                        |

나이, 직업, 교육 수준, 성별, 인종, 출신국가, 자본 상태 등을 통해 소득 수준이 예측 가능할 것이다 