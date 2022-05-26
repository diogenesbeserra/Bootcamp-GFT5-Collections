# Bootcamp-GFT5-Collections-Exemplo1

### Java Collections ArrayList (java.util)

Permite elementos duplicados, indexada - podemos acessar, remover, adicionar, atualizar o elemento de uma posição específica através de seu índice. 

* [x] toString()
* [x] indexOf()
* [x] add()
* [x] set()
* [x] contains()
* [x] get()
* [x] Collections.min()
* [x] Collections.max()
* [x] iterator()
* [x] iterator().hasNext()
* [x] iterator().next()
* [x] size()
* [x] remove()
* [x] iterator().remove()
* [x] clear()
* [x] isEmpty()
 

### Java collections Set - HashSet, LinkedHashSet, TreeSet (java.util)

HashSet - Não permite elementos duplicados, não possui indice, ordem dos elementos aleatória.

LinkedHashSet - elementos na ordemm que são inseridos

TreeSet - elemntos na ordem natural. Crescente ou alfabética

HashSet e LInkedHashSet - permite no máximo um elemento null
TreeSet - não permite elemento null

* [x] toString()
* [x] contains()
* [x] toString()
* [x] Collections.min()
* [x] Collections.max()
* [x] iterator()
* [x] iterator().hasNext()
* [x] iterator().next()
* [x] size()
* [x] remove()
* [x] iterator().remove()
* [x] new LinkedHashMap()
* [x] new TreeMap()
* [x] clear()
* [x] isEmpty()


### Java Colections Map - HashMap, LinkedHashMap, TreeMap

Semelhante ao Set

* [x] toString()
* [x] put()
* [x] containsKey()
* [x] get()
* [x] keySet()
* [x] values
* [x] entrySet();
* [x] getValue();
* [x] getKey();
* [x] iterator()
* [x] iterator().hasNext()
* [x] iterator().next()
* [x] LinkedHashMap()
* [x] new TreeMap()
* [x] clear()
* [x] isEmpty()

### Comparable 

override: 
* [x] ToString
* [x] CompareTo
* [x] HashCode
* [x] Equals

### Comparator

override
* [x] Compare

### Java Collections Streams

Classe Anônima

Classe sem nome que é declarada e instanciada em uma única instrução e é usada apenas uma vez.

Set<Map.Entry<Integer, Contato>> set = new TreeSet<>(Comparator.comparing(
                new Function<Map.Entry<Integer, Contato>, Integer>() {
                    @Override
                    public Integer apply(Map.Entry<Integer, Contato> cont) {
                        return cont.getValue().getNumero();
                    }
                }));


Funcional Interface

interface com um único Método Abstrato: Comparator, Consumer, Function, Predicate

@FunctionalInterface
public interface Comparator<t> {
  @Contract(pure = true) int compare( T var1, T var2);
 }

Função Lambda
 
 Funcção sem declaração, sem nome, sem tipo de retornoe modificador 
 
 (argumento) -> (corpo)
 
 Set<Map.Entry<Integer, Contato>> set = new TreeSet<>(Comparator.comparing(
                cont -> cont.getValue().getNumero()));
 
 
 Reference Method
 
 Faz referência a um método de forma funcional " :: " Simplifica uma Lambda Expression
 
 
 Stream Api
 
* [x] stream - Fluxo de dados que não altera a coleção
* [x] operações intermediárias - Permite operações encadeadas
* [x] operações finais - Fecha o fluxo
* [x] forEach(new Consumer())
* [x] skip()
* [x] collect(Collectors.joining())
* [x] distinct()
* [x] count()
* [x] limit()
* [x] collect(Collectors.toSet())
* [x] map(new Function())
* [x] collect(Collectors.toList())
* [x] filter (new Function())
* [x] sorted()
* [x] mapToInt
* [x] sum()
* [x] average()
* [x] ifPresent()
* [x] min
* [x] max
* [x] removeIf(new Predicate())
* [x] collect(Collectors.groupingBy(new Function())




