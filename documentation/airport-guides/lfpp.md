### About this facility
Paris Orly Airport (LFPO) – one of the two major airports serving the Paris metropolitan area – handles a mix of full-service and low-cost carriers on its dual-runway complex south of the city.

### Airspace & Procedures
* **Vectoring:** Arrivals are vectored off the STAR terminus toward final for runway 25 to manage merges inside the compact Paris terminal area.
* **Departures:** Four RNAV departures are modeled, each with a single exit fix:
  * **Orly Est (EAST)** – feeds traffic through PO243 to BATAG, joining airway AWYDIKOL via the BATAG exit.
  * **Orly Nord (NORTH)** – sequences aircraft via PO243 toward PO262, providing the lone northern exit into airway AWYBOV.
  * **Orly Sud (SOUTH)** – guides jets through PO243 and ADADA before handing them to airway AWYAGOPA at ADADA.
  * **Orly Ouest (WEST)** – turns departures over PO245 and PO191, connecting to airway AWYLGL through the PO191 exit.
* **Arrivals:** Three simplified STARs are available, each with one modeled entry and a common runway 25 terminus where vectoring begins:
  * **CAD1 (Châteaudun)** – flows in from the single CAD entry, stepping down via SOTIP and ODILO before reaching the PO615 initial approach fix.
  * **GITAN1 (Gitan)** – accepts traffic only from the GITAN entry, routing through VEBEK and CTL en route to VALPO.
  * **OKRIX1 (Okrix)** – receives traffic from the OKRIX gate, descending via EBOMA and MOLBA to MLN before the final merge point at PO610.

### Traffic Profile
The scenario uses a realistic 2025 busy-week traffic mix totalling roughly **35 departures and 35 arrivals per hour**, distributed across the modeled airlines and procedures to mirror peak-period demand at Orly.

### Special Considerations: PBN-to-ILS transition
An hypothetical **PBN-to-ILS** approach is modeled for runway 25. Aircraft follow the EMMAQ1 transition to align with the final ILS segment:
* The commands `rr EMMAQ.EMMAQ1.LFPP25` and similar commands fly the full transition and result in an ILS clearance on runway 25
* Controller shortcuts convert direct-to commands into the full routing:
  * `dct EMMAQ ils 25` becomes `rr EMMAQ.EMMAQ1.LFPP25`
  * `dct MEDWY ils 25` becomes `rr MEDWY.EMMAQ1.LFPP25`
  * `dct VEKUH ils 25` becomes `rr VEKUH.EMMAQ1.LFPP25`
