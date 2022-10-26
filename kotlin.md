## Json
* Failed for JSON property author due to missing (therefore NULL) value for creator parameter author which is a non-nullable type
  nullable ?로 변경해본다

* Cannot deserialize instance of `java.util.ArrayList<MyObj>` out of FIELD_NAME token
  클래스명과 필드명이 동일하다면 @JsonProperty("xxx")를 붙여본다 
