---
external help file: PSGateway-help.xml
online version: 
schema: 2.0.0
---

# Invoke-AccountBalance

## SYNOPSIS
Obtiene el balance de las cuentas del cliente.

## SYNTAX

```
Invoke-AccountBalance [[-CorrelationalId] <String>] [-DocType] <String> [-DocNumber] <String>
 [-AccountType] <String> [-AccountNumber] <String> [-AccountPin] <String>
```

## DESCRIPTION
Obtiene el balance con los saldos de las cuentas del cliente.

## EXAMPLES

### -------------------------- EJEMPLO 1 --------------------------
```
Invoke-AccountBalance -DocType 1 -DocNumber 123456789 -AccountNumber 830030924 -AccountType 04 -AccountPin 0000
```

Este ejemplo debe indicar en la respuesta que el cliente no existe.

## PARAMETERS

### -CorrelationalId
Identificador un?voco de la solicitud.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: [System.Guid]::NewGuid().ToString('D')
Accept pipeline input: True (ByValue)
Accept wildcard characters: False
```

### -DocType
Tipo de documento del cliente.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DocNumber
N?mero de identificaci?n del cliente.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AccountType
Tipo de cuenta del cliente.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 4
Default value: (Get-Configuration).Gateway.Transactions.AccountType
Accept pipeline input: False
Accept wildcard characters: False
```

### -AccountNumber
N?mero de la cuenta del cliente.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 5
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AccountPin
PIN de la cuenta del cliente.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

### None

## OUTPUTS

### [Processa.RabbitMQ.Services.Gateway.Contracts.Commands.AccountBalanceBaseResponse

## NOTES
Author: Gabriel Eduardo Duarte Vega

## RELATED LINKS

[[Get-XmlDocumentRequest](Get-XmlDocumentRequest.md)]()

[[Invoke-Gateway](Invoke-Gateway.md)]()

