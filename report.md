レポート課題
===========

### 課題1
新たにswitch_disconnectedメソッドを定義し、スイッチの接続が切れた際にdatapath_idを16進数形式で出力するようにした。
```
  def switch_disconnected(datapath_id)
    logger.info "Bye #{datapath_id.to_hex}!"
  end
```
### 課題2
自クラス名に基づいたメッセージを出力するように既存のstartメソッドを変更した。
自クラス名はself.class.nameにより参照している。
```
  def start(_args)
    logger.info "Hi! from"+self.class.name
  end
```

