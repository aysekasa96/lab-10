# lab-10
# Azure Synapse Analytics Data Pipeline

Dit project heeft tot doel om een gegevenspijplijn (data pipeline) te maken in **Azure Synapse Analytics**. De pijplijn laadt productgegevens van een tekstbestand naar een tabel in een datawarehouse.

## Doel van het Project

Dit project omvat het volgende:
1. Ophalen van brongegevens uit een CSV-bestand in een Azure Data Lake.
2. Verplaatsen van de gegevens naar een tabel in een datawarehouse.
3. Toevoegen van nieuwe producten en bijwerken van bestaande producten.

## Vereisten

- Een Azure-abonnement met beheerdersrechten.
- Een Azure Synapse Analytics-werkruimte:
  - **Data Lake**-koppeling.
  - **SQL Pool** (dedicated SQL pool).

## Projectstructuur

- **Brongegevens**: Het CSV-bestand `Product.csv`.
- **Doel**: De tabel `dbo.DimProduct` in Azure Synapse SQL Pool.
- **Pipeline Stappen**:
  - **Data Flow**: Het verwerken van gegevens uit het bestand.
  - **Lookup**: Controleren op bestaande producten.
  - **Alter Row**: Nieuwe producten toevoegen of bestaande producten bijwerken.
  - **Sink**: Het verwerken van gegevens naar de tabel.

## Gebruik

1. **Aanmelden bij Synapse Studio**:
   - Open Synapse Studio om te beginnen.

2. **Maak een Pipeline**:
   - Maak een nieuwe pipeline op de **Integrate**-pagina en noem deze `Load Product Data`.

3. **Voeg een Data Flow toe**:
   - Maak een data flow genaamd `LoadProductsData`.
   - Stel de bron- en doelgegevenssets in.
   - Configureer de lookup-operatie.

4. **Pipeline Debuggen en Uitvoeren**:
   - Gebruik de **Data flow debug**-functie om de data flow te testen.
   - Voer de pipeline uit om ervoor te zorgen dat de gegevens correct zijn verwerkt.

## Resultaat

Dit project leert hoe je een gegevenspijplijn maakt en beheert die productgegevens naar een datawarehouse laadt. Het is een uitstekend voorbeeld om de data processing-mogelijkheden van Synapse Analytics te ontdekken.





