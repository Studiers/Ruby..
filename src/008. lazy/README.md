# 게으르게 삽시다

부지런하게 살라고 말들하시지만, 그 때 할일은 그때그때 하라고 하시지만 그것은 틀렸습니다!

실은 우리는 실제로 필요할 때 연산하는 것이 좋은 것입니다 ㅇㅅㅇ 아래의 코드를 보시죠

```ruby
(1..Float::INFINITY).map {|n| n}
# ???
```

위의 코드는 멈추지 않습니다, 무한대에 다다르지 못하지만 다다르려고 노력하며 계속 매핑을 진햅합니다 ㅠ

위에서 말한것과 같이 우리는 게을러져야 합니다. 아래의 코드 같이 고쳐봅시다

```ruby
(1..Float::INFINITY).lazy.map {|n| n}
# <Enumerator::Lazy: #<Enumerator::Lazy: 1..Infinity>:map>
```

와우, 이제 매우 게을러(?)졌군요! 바로 Enumberator#Lazy를 리턴했습니다

이제 앞부분의 몇개의 값을 가져와 봅시다. 그때에만 block내의 코드를 실행, 매핑을 진행합니다 CLEAN~~