# Cpf

[![][build-img]][build]
[![][nuget-img]][nuget]

Digit check and formatting on Brazilian Individual Taxpayer Registry ([CPF]).

[build]:     https://ci.appveyor.com/project/TallesL/net-Cpf
[build-img]: https://ci.appveyor.com/api/projects/status/github/tallesl/net-Cpf?svg=true
[nuget]:     https://www.nuget.org/packages/marcos.cpf-validator/
[nuget-img]: https://badge.fury.io/nu/marcos.cpf-validator.svg
[CPF]:       http://en.wikipedia.org/wiki/Cadastro_de_Pessoas_F%C3%ADsicas

## Usage

```cs
using cpfvalidator;

Check.CPF("29594421134");     // True
Check.CPF("488.081.131-91");  // True
Check.CPF("00000000000");     // False
Check.CPF("text");            // False
Check.CPF("");                // False
