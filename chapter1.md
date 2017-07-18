# .vimrc



기본적으로 vim 을 시작하게 되면 로드하게 되는 script 파일은 .vimrc 파일이다.



.vimrc 파일은 시스템마다 로드하는 위치와 순서가 다를 수 있다.



본인의 컴퓨터의 환경에 대해서 살펴보고 싶으면 

``` vim

:version

```

해보면 로드하는 vimrc 에 대한 정보를 알 수 있다. 



조금 더 일반적인 내용에 대해서 보고 싶으면 

``` vim

:help vimrc

```



``` vim

	Places for your personal initializations:

		Unix		$HOME/.vimrc or $HOME/.vim/vimrc

		OS/2		$HOME/.vimrc, $HOME/vimfiles/vimrc

				or $VIM/.vimrc \(or \_vimrc\)

		MS-Windows	$HOME/\_vimrc, $HOME/vimfiles/vimrc

				or $VIM/\_vimrc

		Amiga		s:.vimrc, home:.vimrc, home:vimfiles:vimrc

				or $VIM/.vimrc

```



위와 같이 나온다. 각 시스템에서 어떻게 동작하는지 자세한 설명도 볼 수 있다.



이 처럼 vim 은 뭔가에 대해 궁금할 때 :help something 을 이용하면 원하는 정보를 얻을 수 있다.



vim 에서는 간단히 :e ~/.vimrc 정도만 입력해도 자기 시스템에 맞는 vimrc 를 편집할 수 있다.



앞으로 설명할 스크립트들은 간단히 inline 으로 vim editor 창에 입력해도 되지만, 영구히 저장하고 싶다면 자기 시스템에 맞는 vimrc 파일에 기록하면 된다. 



다음시작 때 부터 vim 은 vimrc 을 읽어들여 실행하게 된다.



``` vim

:echo $MYVIMRC

```

으로도 확인 할 수 있다.





