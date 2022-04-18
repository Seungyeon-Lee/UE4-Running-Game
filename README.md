# UE4-ArenaBattle

[이득우의 언리얼 C++ 게임 개발의 정석] 책을 보고 실습하는 프로젝트입니다.

Unreal Engiene 4.26.2 버전으로 진행.

## CHAPTER 11
- 389p ABCharacter.cpp
- UserWidget(HPBar)의 HP 값이 연동되지 않는 오류

```cpp
	HPBarWidget->InitWidget();
	auto CharacterWidget = Cast<UABCharacterWidget>(HPBarWidget->GetUserWidgetObject());
	if (nullptr != CharacterWidget)
	{
		CharacterWidget->BindCharacterStat(CharacterStat);
	}
```


HPBarWidget->InitWidget(); 추가 [[참고자료](https://mingyu0403.tistory.com/261)]


소스 코드 중 일부 아래의 github 참고하여 수정.

https://github.com/smarthug/UE4-CPP-Book

정오표 http://www.acornpub.co.kr/book/unreal-c#errata


