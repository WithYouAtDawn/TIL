### 주석
- 배경 미리 보여주는 주석
```
@Preview(showBackground = true)
@Composable
fun GreetingPreview() {
    HappyBirthdayTheme {
        Greeting(name: "Compose")
    }
}
```
- 미리보기 제목 사용
```
@Preview(name = "NoXMLYesCompose")
@Composable
fun GreetingPreview() {
    HappyBirthdayTheme {
        Greeting(name: "Compose")
    }
}
```
- 매개변수 X
```
@Preview
@Composable
fun AppleGame() {
    HappyBirthdayTheme{
        Greeting(name: "Compose")
    }
}
```
- 여러 개의 매개변수
```
@preview(
    showBackground = true,
    showSystemUi = true,
    name = "NoXMLYesCompose"
)
@Composable
fun AppleGame() {
    HappyBirthdayTheme{
        Greeting(name: "Compose")
    }
}
```
#### !! 반환하지 않는 @Composable 주석을 단 함수는 파스칼 표기법 !!
- 명사 제외 다 금지
