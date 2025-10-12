# Plagiarism Detection Dataset
## Nuclear Technology Research Applications

This dataset contains examples for teaching LLM-as-judge evaluation. Each example includes a text summary and relevant source material. Your task: determine if the text is **plagiarized** (verbatim or close paraphrase) or **original** (properly paraphrased/synthesized).

**Note:** In real-world applications, you would first use semantic search to retrieve potentially relevant sources. For this exercise, assume retrieval has already been done—all provided sources are topically relevant.

---

## SECTION 1: Labeled Examples for Train/Dev/Test Split
*These 26 examples have ground truth labels. Your first task: strategically split them into training, development, and test sets, ensuring each set has representative variety of plagiarism types and difficulty levels.*

**Recommended split:** ~30% training, ~35% development, ~35% test

**Plagiarism types to look for:**
- Verbatim copying
- Close synonym substitution
- Structural plagiarism (same structure, different words)
- Patchwriting (mixing copied and original phrases)
- Sentence reordering

---

### Example 1
**ID:** labeled_001  
**Difficulty:** easy  
**Label:** plagiarized (verbatim)

**Text:**  
Gamma irradiation is used to sterilize male insects before their release into the environment. The radiation causes chromosomal damage that prevents reproduction while maintaining the insects' ability to mate and compete with wild males.

**Source Text:**  
"Gamma irradiation is used to sterilize male insects before their release into the environment. The radiation causes chromosomal damage that prevents reproduction while maintaining the insects' ability to mate and compete with wild males." (FAO Technical Manual on SIT, 2020)

---

### Example 2
**ID:** labeled_002  
**Difficulty:** easy  
**Label:** original

**Text:**  
The Sterile Insect Technique represents a species-specific and environmentally friendly method of pest control. Male insects are sterilized through irradiation and then released into wild populations. These sterile males compete with wild males for mates, but produce no offspring, leading to population decline over successive generations.

**Source Text:**  
"Sterile Insect Technique (SIT) is an environmentally-friendly insect pest control method involving the mass-rearing and sterilization, using radiation, of a target pest, followed by the systematic area-wide release of the sterile males by air over defined areas. The released sterile insects mate with wild insects of the target population. As there is no offspring, the pest population declines." (IAEA SIT Overview, 2019)

---

### Example 3
**ID:** labeled_003  
**Difficulty:** moderate  
**Label:** plagiarized (structural - same structure, different words)

**Text:**  
Plant mutation breeding employs physical or chemical agents to create genetic variation in agricultural crops. The method has proven especially effective in producing cultivars with improved tolerance to environmental stresses including drought, salt, and temperature extremes. Given the acceleration of climate change, this breeding approach provides a quick method for generating the genetic variability required for crop adaptation.

**Source Text:**  
"Plant mutation breeding uses physical or chemical mutagenic agents to induce genetic variation in crops. This technique has been particularly successful in developing varieties with improved tolerance to abiotic stresses such as drought, salinity, and extreme temperatures. With climate change intensifying, mutation breeding offers a rapid approach to generating the genetic diversity needed for crop adaptation." (Plant Breeding Reviews, 2021)

---

### Example 4
**ID:** labeled_004  
**Difficulty:** moderate  
**Label:** original

**Text:**  
Climate change poses significant challenges to global agriculture, requiring the development of crop varieties that can withstand extreme conditions. Plant breeders utilize mutation induction techniques to accelerate genetic diversity, creating plants with enhanced drought tolerance and disease resistance. These improved varieties help farmers maintain productivity despite increasingly unpredictable weather patterns.

**Source Text:**  
"Plant mutation breeding uses physical or chemical mutagenic agents to induce genetic variation in crops. This technique has been particularly successful in developing varieties with improved tolerance to abiotic stresses such as drought, salinity, and extreme temperatures. With climate change intensifying, mutation breeding offers a rapid approach to generating the genetic diversity needed for crop adaptation." (Plant Breeding Reviews, 2021)

---

### Example 5
**ID:** labeled_005  
**Difficulty:** moderate  
**Label:** plagiarized (synonym substitution)

**Text:**  
Isotopic methods offer important instruments for studying soil moisture movement and nutrient transformation in farming systems. Through monitoring the flow of isotope-tagged materials, scientists can enhance irrigation strategies and fertilizer use, thereby increasing water efficiency and minimizing ecological consequences.

**Source Text:**  
"Isotopic techniques provide valuable tools for understanding soil water dynamics and nutrient cycling in agricultural systems. By tracking the movement of isotopically labeled compounds, researchers can optimize irrigation practices and fertilizer application, ultimately improving water use efficiency and reducing environmental impact." (Soil Science Journal, 2021)

---

### Example 6
**ID:** labeled_006  
**Difficulty:** borderline  
**Label:** original

**Text:**  
Isotopic techniques provide valuable tools for understanding soil water dynamics and nutrient cycling in agricultural systems. By tracking the movement of isotopically labeled compounds, researchers can optimize irrigation practices and fertilizer application, ultimately improving water use efficiency and reducing environmental impact.

**Source Text:**  
"Nuclear and isotopic techniques offer powerful approaches to study water movement in soils and nutrient transformations. These methods involve applying stable or radioactive isotopes as tracers, then monitoring their distribution over time. Data obtained helps scientists develop recommendations for more efficient irrigation scheduling and fertilizer management, leading to reduced water consumption and lower nutrient losses to the environment." (Agricultural Water Management, 2020)

---

### Example 7
**ID:** labeled_007  
**Difficulty:** easy  
**Label:** original

**Text:**  
Food irradiation extends shelf life by reducing microbial contamination without significantly affecting nutritional quality. The process involves exposing food products to controlled doses of ionizing radiation. Consumer acceptance remains a challenge despite extensive safety testing and regulatory approval in many countries.

**Source Text:**  
"Irradiation of food uses ionizing radiation to kill bacteria, viruses, and insects in food products. The technology can increase shelf life and improve food safety. While approved by health authorities worldwide based on decades of research, consumer perception and acceptance vary considerably across different regions and cultures." (Food Safety Magazine, 2020)

---

### Example 8
**ID:** labeled_008  
**Difficulty:** moderate  
**Label:** plagiarized (patchwriting - mixing copied and paraphrased)

**Text:**  
Animal diseases that cross borders pose serious risks to livestock production and human health worldwide. Nuclear and nuclear-derived techniques enable rapid and accurate disease diagnosis, allowing for timely intervention. These diagnostic tools are especially important in developing countries where access to sophisticated laboratory facilities is limited.

**Source Text:**  
"Animal diseases that cross borders pose serious risks to livestock sectors and human health. Molecular diagnostic methods, including those based on nuclear technologies like radioimmunoassay and isotope-labeled probes, provide sensitive and specific detection of pathogens. Such tools are especially important in developing countries where access to sophisticated laboratory facilities is limited." (Veterinary Diagnostics Review, 2021)

---

### Example 9
**ID:** labeled_009  
**Difficulty:** moderate  
**Label:** original

**Text:**  
Transboundary animal diseases represent major threats to livestock production and food security worldwide. Nuclear and nuclear-derived techniques enable rapid and accurate disease diagnosis, allowing for timely intervention and control measures. These diagnostic tools are particularly valuable in resource-limited settings where traditional laboratory infrastructure may be inadequate.

**Source Text:**  
"Animal diseases that cross borders pose serious risks to livestock sectors and human health. Molecular diagnostic methods, including those based on nuclear technologies like radioimmunoassay and isotope-labeled probes, provide sensitive and specific detection of pathogens. Such tools are especially important in developing countries where access to sophisticated laboratory facilities is limited." (Veterinary Diagnostics Review, 2021)

---

### Example 10
**ID:** labeled_010  
**Difficulty:** easy  
**Label:** plagiarized (verbatim)

**Text:**  
The tsetse fly transmits trypanosomiasis, a parasitic disease affecting both humans and livestock in sub-Saharan Africa. Sterile insect technique programs have successfully suppressed or eliminated tsetse populations in several regions. The approach involves mass-rearing, irradiation, and systematic release of sterile males.

**Source Text:**  
"The tsetse fly transmits trypanosomiasis, a parasitic disease affecting both humans and livestock in sub-Saharan Africa. Sterile insect technique programs have successfully suppressed or eliminated tsetse populations in several regions. The approach involves mass-rearing, irradiation, and systematic release of sterile males." (IAEA Tsetse Control Report, 2018)

---

### Example 11
**ID:** labeled_011  
**Difficulty:** moderate  
**Label:** original

**Text:**  
Stable isotope analysis can authenticate the geographic origin of food products by comparing isotopic signatures with reference databases. This technology helps combat food fraud and supports traceability systems in international trade. The method is non-destructive and can be applied to various food matrices including meat, dairy, and produce.

**Source Text:**  
"Food authentication using stable isotope ratio analysis relies on the principle that isotopic composition reflects geographic origin and production methods. By measuring ratios of elements like carbon, nitrogen, oxygen, and hydrogen, and comparing them to reference databases, laboratories can verify product origin claims. This approach supports anti-fraud efforts and trade compliance across diverse food categories." (Food Chemistry, 2020)

---

### Example 12
**ID:** labeled_012  
**Difficulty:** borderline  
**Label:** plagiarized (close paraphrase with partial structure change)

**Text:**  
Nuclear techniques facilitate the detection of pesticide residues and contaminants in food products at trace levels. Mass spectrometry coupled with isotope dilution provides highly accurate quantification, ensuring compliance with international safety standards and protecting consumer health.

**Source Text:**  
"Nuclear-based analytical techniques enable detection of pesticide residues and contaminants in food at very low concentrations. Isotope dilution mass spectrometry offers exceptional accuracy for quantifying these substances, supporting regulatory compliance and consumer protection." (Analytical Chemistry in Food Safety, 2021)

---

### Example 13
**ID:** labeled_013  
**Difficulty:** moderate  
**Label:** original

**Text:**  
Nitrogen-15 isotope studies allow researchers to trace fertilizer uptake efficiency in crops and assess nitrogen losses to the environment. By applying labeled fertilizers, scientists can determine how much nitrogen plants actually absorb versus how much is lost through leaching or volatilization. This information guides recommendations for optimal fertilizer management practices.

**Source Text:**  
"The use of 15N-labeled fertilizers provides direct measurement of nitrogen use efficiency in agricultural systems. Researchers apply fertilizers enriched with the stable isotope nitrogen-15, then track its fate in soil-plant systems. Data reveal the proportion of applied nitrogen taken up by crops compared to amounts lost via various pathways such as leaching to groundwater or gaseous emissions. These findings inform best management practices for nitrogen fertilization." (Nutrient Cycling in Agroecosystems, 2020)

---

### Example 14
**ID:** labeled_014  
**Difficulty:** moderate  
**Label:** plagiarized (sentence reordering with minor changes)

**Text:**  
The process is effective against all insect life stages from eggs to adults, and maintains product quality attributes. Food irradiation provides a non-chemical approach to insect disinfestation in stored commodities and fresh fruits. Growing numbers of countries accept irradiation as a phytosanitary treatment meeting international trade requirements.

**Source Text:**  
"Food irradiation provides a non-chemical approach to insect disinfestation in stored commodities and fresh fruits. The process is effective against all insect life stages from eggs to adults, and maintains product quality attributes. Growing numbers of countries accept irradiation as a phytosanitary treatment meeting international trade requirements." (Radiation Physics and Chemistry, 2019)

---

### Example 15
**ID:** labeled_015  
**Difficulty:** easy  
**Label:** original

**Text:**  
Irradiation technology offers a chemical-free method for controlling insect pests in stored grains and fresh produce. The treatment eliminates insects at all life stages while preserving product quality. International phytosanitary standards increasingly recognize irradiation as an approved quarantine treatment.

**Source Text:**  
"Food irradiation provides a non-chemical approach to insect disinfestation in stored commodities and fresh fruits. The process is effective against all insect life stages from eggs to adults, and maintains product quality attributes. Growing numbers of countries accept irradiation as a phytosanitary treatment meeting international trade requirements." (Radiation Physics and Chemistry, 2019)

---

### Example 16
**ID:** labeled_016  
**Difficulty:** borderline  
**Label:** original

**Text:**  
Soil erosion assessment using fallout radionuclides like cesium-137 provides quantitative data on soil redistribution patterns across agricultural landscapes. This information helps land managers implement targeted conservation measures. The technique is cost-effective compared to conventional erosion monitoring methods.

**Source Text:**  
"Fallout radionuclides, particularly cesium-137, serve as tracers for quantifying soil erosion and redistribution at landscape scales. By measuring the spatial distribution of these isotopes in soil profiles, researchers can reconstruct erosion patterns over recent decades. This approach offers advantages in terms of cost and spatial coverage relative to traditional erosion measurement techniques, informing conservation planning." (Geoderma, 2020)

---

### Example 17
**ID:** labeled_017  
**Difficulty:** moderate  
**Label:** plagiarized (synonym substitution)

**Text:**  
Mass spectrometry combined with isotope dilution offers exceptional precision in measuring food contaminants, supporting regulatory compliance and safeguarding public health.

**Source Text:**  
"Mass spectrometry coupled with isotope dilution provides highly accurate quantification of contaminants in food, ensuring compliance with international safety standards and protecting consumer health." (Analytical Chemistry in Food Safety, 2021)

---

### Example 18
**ID:** labeled_018  
**Difficulty:** easy  
**Label:** original

**Text:**  
The Mediterranean fruit fly poses a serious threat to fruit production worldwide. Area-wide integrated pest management programs combining sterile insect releases with other control methods have achieved remarkable success. Eradication campaigns in several countries have demonstrated the technique's effectiveness when properly implemented.

**Source Text:**  
"Mediterranean fruit fly (Ceratitis capitata) is among the most destructive pests of fruit crops globally. Integrated area-wide management strategies that include sterile insect technique alongside complementary tactics such as lure-and-kill devices and host removal have proven highly effective. Successful eradication programs in countries including Chile, Mexico, and parts of the United States demonstrate that sustained implementation of these integrated approaches can eliminate established populations." (Crop Protection, 2019)

---

### Example 19
**ID:** labeled_019  
**Difficulty:** borderline  
**Label:** plagiarized (patchwriting)

**Text:**  
Nuclear-based diagnostic tools support early detection of livestock diseases, enabling prompt treatment and preventing widespread outbreaks. Such capabilities are particularly critical for transboundary animal diseases that pose risks to food security across multiple countries.

**Source Text:**  
"Diagnostic technologies derived from nuclear science enable rapid identification of livestock pathogens, facilitating timely therapeutic intervention and outbreak containment. Such capabilities are particularly critical for transboundary animal diseases that pose risks to food security across multiple countries." (Transboundary and Emerging Diseases, 2020)

---

### Example 20
**ID:** labeled_020  
**Difficulty:** moderate  
**Label:** original

**Text:**  
Carbon-13 and nitrogen-15 natural abundance measurements distinguish between organic and conventional agricultural products by revealing differences in fertilization practices. Organic systems typically show distinct isotopic patterns reflecting reliance on organic amendments rather than synthetic fertilizers. This approach supports certification and labeling claims in organic food markets.

**Source Text:**  
"Stable isotope ratios of carbon and nitrogen differ between organic and conventional farming systems due to contrasting fertilization regimes. Organic production relies on manures and composts, while conventional systems use synthetic fertilizers, leading to characteristic isotopic signatures in plant tissues. Analysis of these natural abundance patterns provides an objective tool for authenticating organic food products and verifying label claims." (Journal of Agricultural and Food Chemistry, 2020)

---

### Example 21
**ID:** labeled_021  
**Difficulty:** easy  
**Label:** plagiarized (verbatim)

**Text:**  
Food irradiation is a physical treatment that can effectively eliminate pathogenic bacteria such as Salmonella and E. coli from meat products. The process uses ionizing radiation to damage the DNA of microorganisms, rendering them unable to reproduce. International health organizations have endorsed irradiation as a safe food processing technology.

**Source Text:**  
"Food irradiation is a physical treatment that can effectively eliminate pathogenic bacteria such as Salmonella and E. coli from meat products. The process uses ionizing radiation to damage the DNA of microorganisms, rendering them unable to reproduce. International health organizations have endorsed irradiation as a safe food processing technology." (WHO Food Safety Guidelines, 2018)

---

### Example 22
**ID:** labeled_022  
**Difficulty:** borderline  
**Label:** plagiarized (structural with synonym substitution)

**Text:**  
Induced mutations have contributed to the development of numerous crop varieties with improved characteristics including better yield, enhanced disease resistance, and greater tolerance to environmental stress factors.

**Source Text:**  
"Mutation breeding uses ionizing radiation or chemical mutagens to induce genetic variations in plants. This technique has been successfully applied to develop crop varieties with improved traits such as higher yield, disease resistance, and tolerance to environmental stresses." (IAEA Plant Breeding Review, 2019)

---

### Example 23
**ID:** labeled_023  
**Difficulty:** moderate  
**Label:** original

**Text:**  
Real-time PCR assays combined with nuclear techniques provide rapid identification of transboundary animal disease agents, facilitating swift implementation of control strategies. These molecular tools have revolutionized veterinary diagnostics by reducing detection time from days to hours. The technology is particularly valuable during disease outbreaks when quick decisions are critical.

**Source Text:**  
"Molecular diagnostic methods including real-time polymerase chain reaction (PCR), often developed in conjunction with nuclear-derived technologies, enable fast and accurate identification of pathogens causing transboundary animal diseases. These advances have transformed veterinary diagnostic capabilities, shortening turnaround times dramatically compared to traditional methods. Rapid results are especially crucial during disease emergencies when timely decisions on control measures can prevent widespread transmission." (Veterinary Microbiology, 2021)

---

### Example 24
**ID:** labeled_024  
**Difficulty:** moderate  
**Label:** plagiarized (sentence reordering)

**Text:**  
This technology speeds up what would otherwise be a lengthy natural process, producing climate-adapted cultivars in shorter timeframes. Mutation breeding employing nuclear radiation accelerates the generation of genetic diversity in crops, enabling development of varieties with enhanced drought tolerance. Such varieties offer particular benefits to resource-poor farmers cultivating in environmentally stressed areas.

**Source Text:**  
"Mutation breeding employing nuclear radiation accelerates the generation of genetic diversity in crops, enabling development of varieties with enhanced drought tolerance. This technology speeds up what would otherwise be a lengthy natural process, producing climate-adapted cultivars in shorter timeframes. Such varieties offer particular benefits to resource-poor farmers cultivating in environmentally stressed areas." (Crop Science, 2020)

---

### Example 25
**ID:** labeled_025  
**Difficulty:** moderate  
**Label:** original

**Text:**  
Drought-resistant crop varieties developed through mutation breeding help farmers adapt to changing climate conditions and maintain food production. Nuclear techniques accelerate the breeding process by inducing beneficial genetic changes that might take decades to occur naturally. These varieties are particularly important for smallholder farmers in marginal environments.

**Source Text:**  
"Mutation breeding employing nuclear radiation accelerates the generation of genetic diversity in crops, enabling development of varieties with enhanced drought tolerance. This technology speeds up what would otherwise be a lengthy natural process, producing climate-adapted cultivars in shorter timeframes. Such varieties offer particular benefits to resource-poor farmers cultivating in environmentally stressed areas." (Crop Science, 2020)

---

### Example 26
**ID:** labeled_026  
**Difficulty:** borderline  
**Label:** plagiarized (close paraphrase with minimal restructuring)

**Text:**  
Isotopic fingerprinting authenticates food origin by analyzing characteristic isotope ratios that reflect geographic and production conditions. This methodology combats fraudulent labeling and supports traceability in international agricultural trade. The approach has been successfully applied to products ranging from wine and olive oil to meat and honey.

**Source Text:**  
"Isotopic fingerprinting authenticates food origin through analysis of characteristic isotope ratios reflecting geographic and production conditions. This methodology combats fraudulent labeling and supports traceability in international agricultural trade. The approach has been successfully applied to products ranging from wine and olive oil to meat and honey." (Food Control, 2021)

---

## SECTION 2: Unlabeled Examples for Manual Labeling
*Label these 8 examples yourself. This will help you experience the difficulty of creating ground truth and highlight subjectivity on borderline cases. Compare your labels with other participants before the instructor reveals the answer key.*

### Example 27
**ID:** manual_001  
**Difficulty:** borderline  
**Label:** [YOU LABEL THIS]

**Text:**  
Radioimmunoassay methods enable highly sensitive detection of disease pathogens and hormones in animal samples. These techniques employ radioactively labeled antigens or antibodies for quantifying target molecules with exceptional specificity. The technology has proven instrumental in surveillance programs for animal diseases throughout developing nations.

**Source Text:**  
"Radioimmunoassay (RIA) techniques enable sensitive detection of animal disease pathogens and hormones in biological samples. These methods use radioactively labeled antigens or antibodies to quantify target molecules with high specificity. The technology has been instrumental in disease surveillance programs across developing countries." (Veterinary Immunology Methods, 2018)

---

### Example 28
**ID:** manual_002  
**Difficulty:** moderate  
**Label:** [YOU LABEL THIS]

**Text:**  
Neutron activation analysis detects trace elements in soil and plant samples, providing insights into nutrient availability and uptake. The technique involves bombarding samples with neutrons to create radioactive isotopes that emit characteristic gamma rays. This information guides precision agriculture practices and fertilizer recommendations.

**Source Text:**  
"Neutron activation analysis (NAA) is an analytical technique for determining elemental composition of materials. In agricultural applications, samples are irradiated with neutrons, producing radioactive isotopes that emit gamma rays with energies characteristic of specific elements. By measuring these emissions, researchers quantify trace element concentrations in soils and plants, informing nutrient management strategies and precision agriculture." (Nuclear Instruments and Methods, 2019)

---

### Example 29
**ID:** manual_003  
**Difficulty:** borderline  
**Label:** [YOU LABEL THIS]

**Text:**  
More than 3,200 mutant varieties have been officially released globally in over 210 plant species through mutation breeding programs. Major food crops such as rice, wheat, and barley are included, as well as ornamentals and other species. The technique is especially useful for crops where natural genetic variation is limited or where conventional breeding faces biological constraints.

**Source Text:**  
"More than 3,200 mutant varieties have been officially released in over 210 plant species globally through mutation breeding programs. These include major food crops such as rice, wheat, and barley, as well as ornamentals and other species. Mutation breeding is especially useful for crops where natural genetic variation is limited or where conventional breeding is challenging due to biological constraints." (Plant Cell Reports, 2019)

---

### Example 30
**ID:** manual_004  
**Difficulty:** easy  
**Label:** [YOU LABEL THIS]

**Text:**  
The New World screwworm has been successfully eradicated from North and Central America through sustained sterile insect technique programs. Weekly releases of millions of sterile flies created a barrier preventing reinfestation from South America. The program demonstrates how coordinated regional efforts can eliminate major livestock pests.

**Source Text:**  
"New World screwworm (Cochliomyia hominivorax) was eliminated from North and Central America via long-term sterile insect technique campaigns. Programs involved producing and releasing millions of sterile male flies each week, establishing a barrier zone that prevented northward spread from endemic areas in South America. This achievement illustrates the potential of area-wide, multi-country cooperative approaches for permanent pest elimination." (Medical and Veterinary Entomology, 2018)

---

### Example 31
**ID:** manual_005  
**Difficulty:** borderline  
**Label:** [YOU LABEL THIS]

**Text:**  
ELISA-based diagnostic kits provide affordable tools for mass screening in animal disease surveillance, many incorporating reagents produced using nuclear technologies. Field deployment is possible with limited laboratory facilities using these assays. Early disease detection through surveillance programs enables rapid response that limits transmission and economic impacts.

**Source Text:**  
"ELISA-based diagnostic kits, many incorporating reagents produced using nuclear technologies, provide affordable tools for mass screening in animal disease surveillance. These assays are suitable for field deployment with limited laboratory facilities. Surveillance programs using such tests enable early disease detection, facilitating rapid response that limits transmission and economic impacts." (Preventive Veterinary Medicine, 2019)

---

### Example 32
**ID:** manual_006  
**Difficulty:** moderate  
**Label:** [YOU LABEL THIS]

**Text:**  
Rinderpest, once a devastating cattle disease, was eradicated globally in 2011 through coordinated vaccination campaigns supported by nuclear-derived diagnostic tools. The achievement marked only the second disease eradication in history after smallpox. Lessons learned continue to inform control strategies for other transboundary animal diseases.

**Source Text:**  
"Global eradication of rinderpest was declared in 2011, representing the second disease ever eliminated worldwide following smallpox. Success resulted from coordinated international vaccination efforts coupled with surveillance programs utilizing diagnostic techniques including those based on nuclear technologies. Experience gained from the rinderpest campaign provides valuable insights for ongoing efforts against other transboundary livestock diseases." (Veterinary Record, 2012)

---

### Example 33
**ID:** manual_007  
**Difficulty:** borderline  
**Label:** [YOU LABEL THIS]

**Text:**  
Oxygen-18 measurements in plant tissues reveal water use efficiency and drought stress responses under different management practices. Breeders utilize these measurements to identify genotypes with favorable water relations traits. The method offers advantages of being non-destructive and applicable at multiple growth stages.

**Source Text:**  
"Stable isotope ratios of oxygen-18 in plant biomass provide indicators of water use efficiency and plant water status under varying environmental and management conditions. Breeders utilize these measurements to identify genotypes with favorable water relations traits. The method offers advantages of being non-destructive and applicable at multiple growth stages." (Functional Plant Biology, 2020)

---

### Example 34
**ID:** manual_008  
**Difficulty:** easy  
**Label:** [YOU LABEL THIS]

**Text:**  
Isotope hydrology techniques assess groundwater recharge rates and residence times, informing sustainable water resource management in agricultural regions. By measuring tritium, carbon-14, and stable isotopes in water samples, scientists can determine aquifer vulnerability to pollution and over-extraction. This knowledge is essential for protecting irrigation water supplies.

**Source Text:**  
"Isotope hydrology employs environmental isotopes such as tritium, carbon-14, and stable isotopes of hydrogen and oxygen to characterize groundwater systems. These tracers reveal information about recharge rates, water age, and flow patterns. In agricultural contexts, such data help assess aquifer sustainability and vulnerability, supporting management decisions that protect water resources used for irrigation." (Hydrogeology Journal, 2020)

---

## SECTION 3: Production/Evaluation Set (Unlabeled)
*Run your judge on these examples to estimate θ (true success rate). These represent "real-world" unlabeled data.*

### Example 35
**ID:** prod_001  
**Text:**  
African animal trypanosomiasis, transmitted by tsetse flies, constrains livestock productivity across 37 sub-Saharan countries. Integrated control approaches combining sterile insect technique with targets, traps, and trypanocidal drugs offer sustainable solutions. Several countries have achieved local elimination of tsetse populations using these methods.

**Source Text:**  
"Trypanosomiasis transmitted by tsetse flies limits livestock production in 37 countries of sub-Saharan Africa. Sustainable control requires integrated strategies that combine sterile insect technique with other interventions such as insecticide-treated targets and traps, along with chemotherapy. Using such integrated approaches, several nations have successfully eliminated tsetse from defined areas." (PLOS Neglected Tropical Diseases, 2019)

---

### Example 36
**ID:** prod_002  
**Text:**  
Irradiation treatment of food can reduce or eliminate pathogenic microorganisms and parasites, enhancing food safety and extending shelf life. The technology is approved in over 60 countries for various food products. Consumer education remains important for wider acceptance of irradiated foods.

**Source Text:**  
"Food irradiation reduces or eliminates pathogenic microorganisms and parasites, improving food safety and shelf life. More than 60 countries have approved the technology for use on various food products. Despite scientific evidence of safety, consumer acceptance varies, highlighting the need for education initiatives." (Comprehensive Reviews in Food Science and Food Safety, 2020)

---

### Example 37
**ID:** prod_003  
**Text:**  
Fallout radionuclides deposited during atmospheric nuclear testing provide time markers for studying soil erosion and sedimentation processes. Cesium-137 concentrations in soil profiles indicate redistribution patterns over the past 70 years. This retrospective approach complements short-term erosion measurements.

**Source Text:**  
"Fallout radionuclides deposited during atmospheric nuclear testing provide time markers for studying soil erosion and sedimentation processes. Cesium-137 concentrations in soil profiles indicate redistribution patterns over the past 70 years. This retrospective approach complements short-term erosion measurements." (Catena, 2018)

---

### Example 38
**ID:** prod_004  
**Text:**  
Stable isotope techniques can authenticate the geographic origin of food products by comparing isotopic signatures with reference databases. This technology helps combat food fraud and supports traceability systems in international trade.

**Source Text:**  
"Stable isotope analysis can authenticate the geographic origin of food products by comparing isotopic signatures with reference databases. This technology helps combat food fraud and supports traceability systems in international trade. The method is non-destructive and can be applied to various food matrices including meat, dairy, and produce." (Food Chemistry, 2020)

---

### Example 39
**ID:** prod_005  
**Text:**  
Pink bollworm populations in cotton-growing regions of the southwestern United States have been eliminated through area-wide sterile insect releases combined with other management practices. The success required coordination among farmers, researchers, and government agencies across multiple states. Cotton growers now benefit from reduced insecticide use and lower production costs.

**Source Text:**  
"The pink bollworm has been eradicated from cotton production areas in the southwestern United States through integrated area-wide management incorporating sterile insect technique. Success depended on collaborative efforts involving growers, scientists, and regulatory authorities across state boundaries. Elimination of this pest has resulted in decreased reliance on insecticides and improved economic returns for cotton producers." (Journal of Economic Entomology, 2018)

---

### Example 40
**ID:** prod_006  
**Text:**  
The definitive method for quantifying contaminants and adulterants in food samples is isotope dilution mass spectrometry. Precise amounts of isotopically labeled compounds are added as internal standards prior to sample processing. This strategy compensates for matrix interferences and provides accurate measurements across a wide range of food matrices.

**Source Text:**  
"Isotope dilution mass spectrometry is considered the definitive method for quantifying contaminants and adulterants in food samples. The technique involves adding precise amounts of isotopically labeled compounds as internal standards prior to sample processing. This strategy compensates for matrix interferences and provides accurate measurements across a wide range of food matrices." (Analytical and Bioanalytical Chemistry, 2020)

---

### Example 41
**ID:** prod_007  
**Text:**  
Mutation breeding uses radiation or chemical agents to create genetic variations in crops. Breeders then select desirable traits from the resulting mutants. This approach has been used to develop varieties with improved yield, disease resistance, and stress tolerance.

**Source Text:**  
"Mutation breeding employs radiation or chemical mutagens to induce genetic diversity in plant populations. Plant breeders screen the resulting mutant lines for beneficial traits and select individuals with desired characteristics. The methodology has generated numerous improved cultivars exhibiting enhanced productivity, pathogen resistance, and abiotic stress tolerance." (Euphytica, 2019)

---

### Example 42
**ID:** prod_008  
**Text:**  
Enzyme-linked immunosorbent assays utilizing nuclear-derived reagents provide cost-effective tools for screening large animal populations in disease surveillance programs. These diagnostic kits can be used in field settings with minimal laboratory infrastructure. Early detection through surveillance enables timely control measures that prevent disease spread and minimize economic losses.

**Source Text:**  
"ELISA-based diagnostic kits, many incorporating reagents produced using nuclear technologies, provide affordable tools for mass screening in animal disease surveillance. These assays are suitable for field deployment with limited laboratory facilities. Surveillance programs using such tests enable early disease detection, facilitating rapid response that limits transmission and economic impacts." (Preventive Veterinary Medicine, 2019)

---

### Example 43
**ID:** prod_009  
**Text:**  
Stable isotope ratios of oxygen-18 in plant biomass indicate water use efficiency and plant water status under varying conditions. This information helps breeders select genotypes with superior water-saving characteristics. The technique is non-invasive and can be applied throughout the growing season.

**Source Text:**  
"Stable isotope ratios of oxygen-18 in plant biomass provide indicators of water use efficiency and plant water status under varying environmental and management conditions. Breeders utilize these measurements to identify genotypes with favorable water relations traits. The method offers advantages of being non-destructive and applicable at multiple growth stages." (Functional Plant Biology, 2020)
