# AndroidLocalBroadcastManagerSample

LocalBroadcastReceiverって特定条件では意外と使えるということを確認するサンプル。
Activityから、5秒のTimerをIntentServiceで開始し、5秒後にLocalBroadcastReceiverでIntentServiceの結果を受け取る。
画面回転をしても、結果自体は正常に受け取れることを確認できる。
ただしActivityが破棄されてしまうと結果を受け取れない。開発者オプションで「アクティビティを保持しない」をTrueにして、IntentService実行中にホームボタンを押して挙動を確かめられる。
