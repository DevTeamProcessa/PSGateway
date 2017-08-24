---
external help file: PSGateway-help.xml
online version: 
schema: 2.0.0
---

# Register-LogEntry

## SYNOPSIS
Crea un nuevo registro de log.

## SYNTAX

```
Register-LogEntry [-ServerName] <String> [[-EventLogLevel] <EnumLogginEventLevel>] [[-SourcePath] <String>]
 [-AppName] <String> [-OperationName] <String> [[-AdjunctFields] <Object>] [-Summary] <String>
```

## DESCRIPTION
Registra una nueva entrada de log del tipo especificado (EventLogLevel).

## EXAMPLES

### -------------------------- EJEMPLO 1 --------------------------
```
El siguiente ejemplo registra una nueva entrada de log de tipo 0-Information
```

Register-LogEntry -EventLogLevel 0 -ServerName $env:computername -AppName 'GatewayMobile' -OperationName 'Get-Token'  -Summary $errorMessage

## PARAMETERS

### -ServerName
Nombre del servidor que origina el registro de log.

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

### -EventLogLevel
Tipo de registro: 0-Information | 1=Warning | 2=Error

```yaml
Type: EnumLogginEventLevel
Parameter Sets: (All)
Aliases: 
Accepted values: Information, Warning, Error

Required: False
Position: 2
Default value: Information
Accept pipeline input: False
Accept wildcard characters: False
```

### -SourcePath
Ruta de la aplicación que origina el registro de log.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AppName
Nombre de la aplicación que origina el registro de log.

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

### -OperationName
Nombre de la operación/acción que origina el registro de log.

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

### -AdjunctFields
Información complementaria al evento.

```yaml
Type: Object
Parameter Sets: (All)
Aliases: 

Required: False
Position: 6
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Summary
Mensaje descriptivo del evento.

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

## INPUTS

## OUTPUTS

### [System.Object]

## NOTES
Author: Jairo Espitia

## RELATED LINKS

