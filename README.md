# sokoban
程式構想：
	輸出地圖：用字元陣列排好地圖的樣子(包含玩家起始位子、箱子、終點)
	移動判斷：讀到相對應鍵值時，判斷下一個位子是否可以移動
	箱子判斷：讀到相對應鍵值時，判斷下一個位子是否可以移動，不能同時推兩個箱子
	終點判斷：當箱子推到終點時改變其字元
	過關：所有箱子都推到終點即過關
	選單：讓玩家可以選擇關卡或退出遊戲
	遊戲中回到選單：按ESC鍵可以回到選單
	過關切換：完成關卡時有個切換場景並跳到下一關
	時間：紀錄完成一關所花的時間

	Main：輸出初始畫面、規則、選單、讀鍵值跳到相對應的函式作處理；判斷是否過關、換地圖
	TimerScore：刷新時間
	UpMove、DownMove、RightMove、LeftMove：判斷要移動的下一個位子是什麼，若是空白把下一個位子改成玩家，上一個位子改成空白；若是牆壁，則不可移動；若是箱子則看箱子的下一個位子能不能移動，可以的話同時移動；若是箱子移到終點，將字元改變表示成功；不能同時推兩個以上箱子
	Draw：把字元陣列輸出
	TimerCount：算時間
	DrawTitle：輸出初始畫面

初始畫面按下Enter後進入規則說明，再按下Enter進入選單，輸入數字(1~6)決定關卡或是退出遊戲，進入遊戲畫面後以上下左右鍵控制A，把O推到*處及通關，#是障壁，過關時會出現YOU WIN!!!字樣，並顯示所花的時間，程式會自動切換到下一關。遊戲中只要按下ECS鍵即可退回到選單。
