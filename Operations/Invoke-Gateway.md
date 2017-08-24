---
external help file: PSGateway-help.xml
online version: 
schema: 2.0.0
---

# Invoke-Gateway

## SYNOPSIS
Invoca operaci?n y actualiza contrato de respuesta con informaci?n de Gateway.

## SYNTAX

```
Invoke-Gateway [-CorrelationalId] <String> [-TypeName] <String> [-XmlRequest] <XmlDocument>
```

## DESCRIPTION
Invoca operaci?n y actualiza contrato de respuesta con informaci?n de Gateway.

## EXAMPLES

### -------------------------- EJEMPLO 1 --------------------------
```
El siguiente ejemplo actualiza el contrato de respuesta con la informaci?n de Gateway.
```

Invoke-Gateway -TypeName $MyInvocation.MyCommand.OutputType.Name -CorrelationalId $CorrelationalId -XmlRequestInnerXml $XmlRequest.InnerXml

## PARAMETERS

### -CorrelationalId
Identificador correlacional un?voco con el que se desea identificar la solicitud.

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

### -TypeName
Tipo de objeto que se utilizar?
para realizar la solicitud.

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

### -XmlRequest
Documento XML de solicitud.

```yaml
Type: XmlDocument
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
Author:         Gabriel Eduardo Duarte Vega
Creation Date:  2017-08-08
Purpose/Change: Versi?n inicial

## RELATED LINKS

