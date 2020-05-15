# README

## Story

Adventure is a CLI game. The player has to explore in the castle with many levels and a lot of rooms. The task of the player is to find a room where the princess is prisoned and take her leave the castle. There are many types of rooms, and each type of room has different types of exits. Note that there's a monster in one of the rooms, which the exact location is not able to be aware. But once the player meets a monster, the game is over.

When the game starts, the player is in the lobby of the castle. Then the program shows information about the lobby：name of the room, how many exits are there, and names of all exits (e.g.: "east", "south", "up"), like:

```
Welcome to the lobby. There are 3 exits: east, west and up.
Enter your command:
```

The player then can input "go" followed by the name of one exit to enter the room connected to that door, like:

```
go east
```

The player goes into the room to the east. The program shows the information about that room, like what happened in the lobby just now. And the player may input command to choose another room.

Once the player enters a room with a monster, the program shows a message and game over. Once the player enters the room of princess, the program shows a message about the princess, and the princess is going to leave with the player. The player then has to find their way out the castle. The only way to leave the castle is via the lobby.

All printed messages and user input are in English to simplify the code.

## Evaluation standard

1. c++ code quality (clean, compact and reasonable)
2. comments quality
3. at least three different kinds of rooms
4. at least five rooms
5. the room with monster or princess is randomly set

## 程序说明
1.打开.exe文件，如果打开失败，可能需要使用vs2019进行重新编译
2.根据游戏提示输入游戏的level与exitPercent
	level		|	新房间中princess与monster出现的概率设定
	exitPercent	|	新房间中出口存在概率设定
3.文件中.cpp与.h头文件一一对应
4.游戏不需要额外的文件进行输入，房间属性由工程内部随机决定

## CopyRight

  *FileName:		MyAdventure
  *Author:		Miracle_Zero
  *Date:		2020/3/28


## 任务需求

1. 第一个房间lobby保证没有公主或怪兽
2. 公主与怪兽不出现在同一个房间
3. 每次进入新房间时随机生成一个房间，一定概率出现公主或怪兽，概率大小可以取决于游戏难度level
4. 新生成一个房间时，随机生成它的出口
5. 来时的出口的对面出口必然是房间的出口
6. 遇见怪兽游戏结束
7. 遇见公主需将公主带回lobby
   
1. The first room lobby guarantees no princesses or monsters
2. The princess and the monster do not appear in the same room

3. Each time you enter a new room, a room is randomly generated. 
   A princess or monster will appear with a certain probability. The probability can depend on the difficulty level
4. When a new room is generated, randomly generate its exit
5. The exit opposite to the exit when coming must be the exit of the room
6. Meet monsters game over
7. Meet the princess and bring the princess back to the lobby
