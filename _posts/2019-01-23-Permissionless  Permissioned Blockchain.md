# Permissionless / Permissioned Blockchain

  Blockchain Platform에는 여러 종류가 있다. 그 중에서 permissionless와 permissioned blockchain의 차이는 무엇인지 알아보자.

  Permissionless Blockchain은 블록체인 네트워크에 어느 누구나 참여할 수 있다는 특징을 가지고 있다. 노드를 구성하여 참여해도 되고, 개발자는 해당 플랫폼의 기능을 개선하거나 해당 플랫폼 기반의 새로운 서비스를 구축할 수 있다. Permissionless Blockchain에서는 블록체인 네트워크에 참여하는 참여자들 모두 익명이므로, 참여자 간 신뢰 관계가 없다. 신뢰 관계가 없는 것을 완화하고자, Mining 또는 Transaction Fee를 두는 경우가 많다. Permissionless Blockchain의 가장 큰 예로는 Bitcoin Core, Ethereum이 있다. 

  그에 반해, Permissioned Blockchain은 블록체인 네트워크에 어느 누구나 참여할 수는 없다. 즉, 일정 수준의 신뢰를 얻은 심사된, 허가된 사용자만 참여할 수 있다는 큰 특징이 있다.  Permissioned Blockchain은 대가가 큰 Mining을 필요로 하지 않는, CFT나 BFT 계열의 합의 알고리즘을 사용하는 블록체인이며, 네트워크에 참여하는 모든 참가자의 행위들 (Invoke Transaction, Deploy Chaincode)을 모두 알 수 있기 때문에 스마트 컨트랙트에 악의적인 코드를 의도적으로 넣는 공격에 대한 위험도 줄어들게 되었다. Permissioned Blockchain의 가장 큰 예로는 리눅스 재단에서 주관하는 Hyperledger 가 있다.