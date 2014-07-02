#Sublime text2　設定懶人包

請先安裝好Sublime Text2，在Ubuntu下可用下列步驟安裝

	sudo add-apt-repository ppa:webupd8team/sublime-text-2
	sudo apt-get update
	sudo apt-get install sublime-text

[出處](http://askubuntu.com/questions/172698/how-do-i-install-sublime-text-2)

###安裝Packet Manerger
* 套件的網址 [https://sublime.wbond.net/](https://sublime.wbond.net/)
* 按下ctrl+`並輸入

		import urllib2,os,hashlib; h = '7183a2d3e96f11eeadd761d777e62404' + 'e330c659d4bb41d3bdf022e94cab3cd0'; pf = 'Package Control.sublime-package'; ipp = sublime.installed_packages_path(); os.makedirs( ipp ) if not os.path.exists(ipp) else None; urllib2.install_opener( urllib2.build_opener( urllib2.ProxyHandler()) ); by = urllib2.urlopen( 'http://sublime.wbond.net/' + pf.replace(' ', '%20')).read(); dh = hashlib.sha256(by).hexdigest(); open( os.path.join( ipp, pf), 'wb' ).write(by) if dh == h else None; print('Error validating download (got %s instead of %s), please try manual install' % (dh, h) if dh != h else 'Please restart Sublime Text to finish installation')

* 重開 sublime text

###安裝套件###
* 按下 ctrl+shift+p
* 輸入 `install` 
* 輸入 套件名稱

###常用套件###
* ApplySyntax 自動偵測語言調整與法Hight Light
* Emmet 原Zen Coding，自動產生HTML標籤
* ConvertToUTF8 處理Big5編碼檔案用
* Git
* HTML-CSS-JS Prettify　自動格式化程式碼（需搭配Node.js）　
* SublimeCodeIntel程式碼自動追蹤工具，追蹤Function定義位置，安裝後按下ctrl+點function就會自動跳到定義。
* Theme-Soda　外觀。
* Sub­limeLin­ter 寫JS以及CSS的神兵利器。
* Phpcs 寫PHP的程式碼輔助。
* Alignment 程式碼對齊，安裝後選取程式碼按ctrl+alt+a。
* WordHighlight 讓選取PHP變數時候會一起選擇$字號

### 不常用套件###
* SFTP 
* Hyperion for gettext 語系檔（*.po)上色
* Color Highlighter 顏色標簽上色
* SublimeBlockCursor 覺得游標還是太小的話，可以裝這個。
* BracketHighlighter 清楚標出括弧的範圍
* Stupid Indent 自動排版用


##Windows 7設定右鍵開啟
請下載　[https://gist.github.com/iaian/5265136/download
](https://gist.github.com/iaian/5265136/download)

解壓縮後會有個reg檔，執行後就能使用右鍵開啟



##界面設定

		Preferences > Settings - User

標記游標所在處

* "highlight_line": true,

標記修改過尚未儲存的檔案

* "highlight_modified_tabs": true,


把TAB轉成空白

* "translate_tabs_to_spaces": true,

游標變胖

* "wide_caret": true,

##常用熱鍵

詳細版
[http://www.camdemy.com/media/6211](http://www.camdemy.com/media/6211)

		Ctrl + / 註解或取消註解
		Ctrl + Shift + V 貼上並符合縮排
		Ctrl + Shift + P 下指令