[![Build status](https://ci.appveyor.com/api/projects/status/r9ovipu6yu7numn6?svg=true)](https://ci.appveyor.com/project/carloscds/boleto2net)
[![Nuget count](http://img.shields.io/nuget/v/Boleto2.Net.svg)](http://www.nuget.org/packages/Boleto2.Net/)
[![Issues open](https://img.shields.io/github/issues/BoletoNet/boleto2net.svg)](https://huboard.com/BoletoNet/boleto2net/)
[![Coverage Status](https://coveralls.io/repos/github/BoletoNet/boleto2net/badge.svg?branch=master)](https://coveralls.io/github/BoletoNet/boleto2net?branch=master)

# boleto2net para .NET CORE 2.2
Fork da Nova versão do Boleto.Net com as seguintes alterações fundamentais:
*  Sem .resx => Nova estrutura de arquivos 
*  Suporte a PDF Nativo em projeto separado boleto2net.pdf - Biblioteca PDF embarcada (wkhtmltopdf.exe)
*  Netstandard 2.2
*  Nenhuma dependência de controles do da System.Web
*  Compliance com a Boleto2NetProxy

### Carteiras Homologadas
* Banrisul - Carteira 1
* Bradesco - Carteira 09
* Brasil - Carteira 17 (Variações 019 027)
* Caixa Econômica Federal - Carteira SIG14
* Itau - Carteira 109, 112
* Safra - Carteira 1
* Santander - Carteira 101
* Sicoob - Carteira 1-01

### Carteiras Implementadas (Não foi homologada. Falta teste unitário)
* Banco do Brasil Carteira 11 (Variação 019)

> Atenção: Para manter a ordem do projeto, qualquer solicitação de Pull Request de um novo banco ou carteira implementada, deverá seguir o formato dos bancos/carteiras já implementados e vir acompanhado de teste unitário da geração do boleto (PDF), arquivo remessa e geração de 9 boletos, com dígitos da linha digitável variando de 1 a 9, checando além do próprio dígito verificador, o cálculo do nosso número, linha digitável e código de barras.

### Como migrar do Boleto.Net
https://github.com/BoletoNet/boleto2net/blob/master/migracao.md

### Night Builds - Build gerado a cada commit do repositorio
Você pode adicionar a URL abaixo no seu Visual Studio mas opções de Pacote do Nuget:
https://www.myget.org/F/boleto2netbuild/api/v3/index.json

### Pre requisitos
Visual Studio 2017 ou superior
