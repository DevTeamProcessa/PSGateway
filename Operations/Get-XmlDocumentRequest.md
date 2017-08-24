---
external help file: PSGateway-help.xml
online version: 
schema: 2.0.0
---

# Get-XmlDocumentRequest

## SYNOPSIS
Retorna documento XML de solicitud generica al servicio de Gateway de tipo \<genericDebitAndCreditCard\>.

## SYNTAX

```
Get-XmlDocumentRequest [-CorrelationalId] <String> [-DocType] <String> [-DocNumber] <String>
 [-AccountNumber] <String> [-AccountType] <String> [-AccountPin] <String> [-TranType] <String>
 [[-ExtTranType] <String>]
```

## DESCRIPTION
Se genera un documento XML a partir de la plantilla y se actualizan los datos correspondientes para la nueva solicitud al servicio de Gateway.

## EXAMPLES

### -------------------------- EJEMPLO 1 --------------------------
```
Get-XmlDocumentRequest -TranType 51 -DocType 4 -DocNumber 123456789 -AccountNumber 830030924 -AccountType 04 -AccountPin 0000 -Amount 999,999.99
```

En el siguiente ejemplo dar?
como resultado un documento XML con la estructura para realizar una solicitud al Gateway.

## PARAMETERS

### -CorrelationalId
Identificador un?voco de la solicitud.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
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

### -AccountNumber
N?mero de la cuenta del cliente.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 4
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

### -TranType
Tipo de transacci?n en \<genericDebitAndCreditCard\>

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 7
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExtTranType
Tipo extendido de transacci?n en \<genericDebitAndCreditCard\>

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 8
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

### [System.Xml.XmlDocument]

## NOTES
Author:         Gabriel Eduardo Duarte Vega
Creation Date:  2017-08-08
Purpose/Change: Versi?n inicial

## RELATED LINKS

