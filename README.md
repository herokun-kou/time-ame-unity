# Time Ame Unity

<img src="https://github.com/herokun-kou/time-ame-unity/blob/master/Screenshots/default_preferences.png" width="100%" title="main screen with default preferences"/>

<img src="https://github.com/herokun-kou/time-ame-unity/blob/master/Screenshots/decorated.png" width="100%" title="main screen with decorated preferences"/>
   
Wallpaper Engine에 붙히는 배경화면용 시계 프로그램.   
시계, 배경, 배경의 밝기효과, 제목, 부제목이 전부입니다.   
시계와 배경을 제외한 요소들은 선택적요소이며 사용하지 않을 수 있습니다.   


## Preferences
   
해당 어플리케이션은 다음 7가지 설정 요소를 갖추고 있습니다.   
- 제목(title) : 화면 좌측의 두 줄 텍스트 중 윗줄의 텍스트를 정합니다.
- 부제목(subtitle) : 화면 좌측의 두 줄 텍스트 중 아랫줄의 텍스트를 정합니다.
- 배경이미지 이름(background) : 배경이미지의 파일명을 정합니다. 확장명을 포함해야합니다. 배열 형태로 주어지며 배열의 항목이 하나인 경우 무조건 해당 이미지로, 둘 이상인 경우 그 중 하나를 랜덤하게 선택합니다.
- 밝은 배경이미지 이름(background_bright) : 밝은 배경이미지의 파일명을 정합니다. 이 또한 확장명을 포함해야 하며, 없는 파일이름으로 정하면 사용안함 모드가 됩니다. 마찬가지로 배열 형태로 주어지며 배경 이미지와 같은 순서로 지정해야 합니다.
- 시계 가로 좌표(clock_x)와 시계 세로 좌표(clock_y) : 시계의 위치를 정합니다.
- 텍스트 영역 가로 좌표(text_x)와 텍스트 영역 세로 좌표(text_y) : 텍스트의 위치를 정합니다.
- 제목 오프셋(title_offset)과 부제목 오프셋(subtitle_offset) : 제목의 세로 좌표와 부제목의 세로 좌표를 각각 정합니다. 제목이나 부제목의 텍스트가 길 경우 사용하면 효과적입니다.
   
위의 설정들을 json문법에 맞게 (실행파일위치)/Preferences/prefs.json 파일에 저장하면 설정이 반영됩니다.   
예시는 아래와 같습니다.   
```json
{
	"title":"public class HeroKun extends Person { ... }",
	"subtitle":"마음만은 언제까지나 멍멍이 소년",
	"background":["background.png", "background_2.png"],
	"background_bright":["background_bright.png", "background_2_bright.png"],
	"clock_x":"4.5",
	"clock_y":"-0.05",
	"text_x":"-4.5",
	"text_y":"0",
	"title_offset":"0.15",
	"subtitle_offset":"-0.15"
}
```
* 밝은 배경이미지에 대해   
밝기 애니메이션을 위한 옵션이며, 정상적으로 설정시 배경 이미지 위에 밝은 배경 이미지가 페이드 인/아웃 효과를 통해 천천히 깜빡입니다.   
포토샵 등의 프로그램으로 명도 등의 조정을 주고 저장하여 설정했을 때 최적의 효과를 발휘합니다.   

## Downloads
   
해당 프로그램의 다운로드는 이쪽에서 가능합니다 :   
[Download : Google Drive](https://drive.google.com/open?id=1SUuYrNBGbNENJS09ASBcAsWmnmiM9ZC3)   

### 패치노트
2020-05-02, 15:06 : 배경 이미지를 랜덤 선택하는 기능이 추가되었고, 배경 이미지 출력 크기가 고정되어 이미지의 크기와 다르게 설정되면 이미지가 눌리던 현상이 수정되었습니다.   
2020-02-09, 18:50 : 어플리케이션이 일시 중지되었다가 다시 실행되면서 시간이 변경될 때 이전 시간에 표시되었던 숫자의 알파값이 정상적으로 내려가지 않던 문제 수정.   
2020-02-10, 18:15 : 요소들의 위치에 대한 설정이 추가되었습니다.

