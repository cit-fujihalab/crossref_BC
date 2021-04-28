# Experimental implementation of the cross-referencing method forscalable public blockchain

The program is in the process of being created

## Dependency/Setup [使い方と開発環境]
Ubuntu 20.04.2 LTS
 - Python3.8

Module list
~~~
 - $ pip3 install websocket_server
 - $ pip3 install websocket_client
 - $ pip3 install pycryptodome
~~~


## Usage　[実行方法]
I will explain the needs in the execution method and startup order by Ubunutu(Linux).

-----------

Ubunutuによる実行方法と起動順番にニードの説明をする。

 ### $ python3 owner_server1.py
 - Start owner_server1.py of Layer-0 primitive central core node.
 - At the same time, the Layer-1 node connection is also started.

--------

 - Layer-0の原始中心コアノードのowner_server1.pyを起動。
 - Layer-1のノードコネクションも同時に起動される。

 ### $ python3 owner_server3.py
 - Node activation that cooperates with the history crossing method that is not the primitive node of Layer-0.
 - By increasing owner_server3.py to an arbitrary number of Layer-0 nodes (number of domains) involved in the history crossing method can be increased.

--------

 - Layer-0の原始ノードではない履歴交差法に協力するノード起動。
 - owner_server3.pyを任意にの数に増やすことで履歴交差法に関わるLayer-0のノードの数（ドメインの数）を増やすことができる。


 ### $ python3 owner_server2.py
 - Layer-0 Command Node
 - Request each domain to take command at Layer-0 and start the history crossing method.

--------

 - Layer-0の統率ノード
 - Layer-0で統率を取り履歴交差法を開始する依頼を各ドメインに出す.

---------
Add after updating...
