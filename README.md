# sound_IO
coralboardとスマホだけの電子制御
PCを持たずともマイコン制御ができたら便利だと思い設計を考えました。
# 使用環境
coralboard :最新のGoolgleが出す超省エネ性が高いgemma3 270mなどを動かすためのボード

スマホ      :これは音声操作とスマホからの操作も対応


<img width="602" height="1097" alt="image" src="https://github.com/user-attachments/assets/cd3e5ea4-6813-4e3b-8453-80d12dacfe16" />



これはスマホで音声認識(Fastwhisper)をスマホ側で行い、そのテキストエディタをCoral boardがどの環境でも動くようにブルートゥースで受け取ってGemma3で判断、物理的な(GPIO、PWM、UART)を行うというパイプラインを構築しています。
これにより、モバイルバッテリー駆動という物理的制約下でも、クラウド並の応答速度と高い操作性を両立させる設計を考えています。

