---
layout: post
title: Como fazer posts minimalistas
---

O spring framework é basicamente um framework open-source Java de injeção de dependência e inversão de controle. E isso é feito em tempo de runtime. Esses são os seus dois principais princípios. Sua principal função é criar objetos e popular as suas dependêcias. Resumindo, o Spring é um framework de injeção de dependência que promove um baixo acoplamento do código através da inversão de dependência.

Seus principais conceitos são:

- **Beans**: São objetos das classes gerenciadas pelo Spring. Anotações como `@Component`, `@Repository` e `@Service` são classes que o Spring fica responsável por instanciá-las após injetar as devidas dependências.
- **Autowiring**:É o processo de identificar uma dependência, buscar um correspondente, e injetar a dependência. A anotação `@Autowire` indica para o Spring para achar e injetar um Bean no outro.
- **Dependency Injection**: É o processo em si de _autowiring_. O Spring pode fazer isso através da injeção via construtor da classe, no setter ou propriedade.
- **Inversion of Control**: O Spring fica responsável por procurar o objeto, criá-lo e injetá-lo dentro da classe. Tradicionalmente, a classe instancia dentro dela o objeto necessário, gerando um alto acoplamento. Com o Spring, essa responsabilidade do controle fica invertida. Basta a classe definir a necessidade de certa dependência para o framework, realizando o processo de _dependency injection_.
- **IoC Container**: É o framework que permite o _inversion of control_. Esse container gerencia os _beans_. Ele é implementado de duas formas no Spring: _Bean Factory_ ou _Application Context_. Por padrão ele utilizará o _Application Context_, mas caso tenha alguma limitação de memória, o _Bean Factory_ deverá ser utilizado.
- **Bean Factory**: é a versão mais simples do _ioc container_. Ele ainda existe por questões de compatibilidade com versões antigos ou para usos onde há restrição de memória.
- **Application Context**: é a versão atual do _ioc container_. Parte principal do framework, onde toda a lógica do Spring acontece. Possui algumas funções adicionais como o Spring AOP, internacionalização, web application context e dentre outros.

