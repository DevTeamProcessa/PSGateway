---
external help file: PSGateway-help.xml
online version: 
schema: 2.0.0
---

# Register-TransactionLog

## SYNOPSIS
Registra la respuesta del microservicio en el log informativo.

## SYNTAX

```
Register-TransactionLog [-ResponseContract] <Object> [-OperationName] <String> [-CmdLetLine] <String>
```

## DESCRIPTION
Registra la respuesta del microservicio en el log informativo d Processa, antes de finalizar la ejecuci?n de la transacci?n.

## EXAMPLES

### -------------------------- EJEMPLO 1 --------------------------
```
El siguiente ejemplo registra la respuesta del microservicio en el log informativo.
```

Register-TransactionResponse -ResponseContract $Response -CmdletInvocation $CmdletInvocation

## PARAMETERS

### -ResponseContract
Objeto de contrato de respuesta.

```yaml
Type: Object
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -OperationName
{{Fill OperationName Description}}

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

### -CmdLetLine
String descriptivo de la invocaci?n del comando de transacci?n (nombre y par?metros).

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

## INPUTS

## OUTPUTS

## NOTES
Author:         jespitia
Creation Date:  11/04/2017
Purpose/Change: Versi?n inicial

## RELATED LINKS

