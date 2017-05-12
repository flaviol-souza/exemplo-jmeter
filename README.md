# exemplo-jmeter: exemplos simples de JMeter para aulas

## Exemplos:
* **command-line**: plano de testes para execução do JMeter vinha linha de comando, como em casos onde a aplicação testada não é Java;
* **maven**: exemplo de aplicação maven, utilizando o [jmeter-maven-plugin](https://github.com/jmeter-maven-plugin/jmeter-maven-plugin);

## command-line
### Pré-requisitos:
* Instalar e configurar corretamente o Java 1.8;
* Instalar o [JMeter 3.2](http://jmeter.apache.org/download_jmeter.cgi) e incluir o diretório `$JMETER_HOME/bin` no `PATH` do sistema;

### Como executar:
Num prompt/shell, digitar:
``` shell
jmeter -n -t command-line/consulta-google-jmeter-3.2.jmx -l resultado.jtl -e -o ./output
```

## maven
### Pré-requisitos:
* Instalar e configurar corretamente o Java 1.8;
* Instalar o [Apache Maven 3.5.0](https://maven.apache.org/download.cgi) e incluir o diretório `$MAVEN_HOME/bin` no `PATH` do sistema;

### Como executar:
Num prompt/shell, digitar dentro do diretório `exemplo-jmeter/maven/`:
``` shell
mvn verify
```
