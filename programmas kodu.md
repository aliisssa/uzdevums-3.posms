# Sistēmas koncepcija
class MedicinsVards:
    def __init__(self, pacients, aizsardziba, vardu_vecums):
        self.pacients = pacients
        self.aizsardziba = aizsardziba
        self.vardu_vecums = vardu_vecums

# Aizsargātas elektroniskās medicīniskās kartes izstrāde
class ElektroniskaKarte:
    def __init__(self, pacients, medicins_vards, veselības_vēsture, konsultācijas):
        self.pacients = pacients
        self.medicins_vards = medicins_vards
        self.veselības_vēsture = veselības_vēsture
        self.konsultācijas = konsultācijas

# Mobilās aplikācijas izstrāde
class MobiloAplikacja:
    def __init__(self, pacients, elektroniska_karte, aplikācijas_dizains, funkcionalitāte):
        self.pacients = pacients
        self.elektroniska_karte = elektroniska_karte
        self.aplikācijas_dizains = aplikācijas_dizains
        self.funkcionalitāte = funkcionalitāte

# Projekta rezultātu apraksts
projekta_rezultati = {
    "specifikācija": {
        "sistēma": "MedicīnsVards",
        "kartes_izstrāde": "ElektroniskaKarte",
        "mobilās_aplikācijas": "MobiloAplikacja"
    },
    "izstrādes_plāns": {
        "koncepcijas_izstrāde": 1,
        "prototipa_izveide": 2,
        "kartes_izstrāde": 4,
        "mobilās_aplikācijas": 3,
        "testēšana_un_drošības_uzlabošana": 2,
        "palaišana_un_tālummaiņa": 2
    },
    "uzdevuma_tehniskā_specifikācija": "Konceptuāla piemērojamība, lietotāju pētījumu atbilstība, tehniskā prasāmība atbilstība",
    "izvirzīto_mērķu_izpildes_līmenis": 80,
    "lēmuma_aktualitāte": "Veicināti izmaiņas, kas ļauj iemīļot veselības sistēmas jaunumu un pievienot savu prasmju izpildi."
}
