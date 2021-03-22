![image](https://user-images.githubusercontent.com/56414953/112048508-deeba200-8b24-11eb-8cfa-9b61476acc04.png)
# Covid-19 Final Project Introduction
In this report, SARS-CoV-2 symptoms, lifecycle, testing, and vaccines are explaind followed by charts covering the pandemic test, case, recovery, death, and vaccination totals. This report uses a logit model to determine the log odds relationship between government covid-19 preventative regulations and cases of SARS-CoV-2. Then, this report uses time-series modeling to determine the progression of the pandemic.
# Covid-19 General Information
A new type of coronavirus, SARS-CoV-2, started in December 2019 and has caused the COVID-19 global pandemic. SARS-CoV-2 originated in a Chinese city called Wuhan. Coronaviruses are common in animals, and scientists hypothesize that SARS-CoV-2 may have transfered to humans, zoonosis, through the Wuhan food market. SARS stands for severe acute respiratory syndrome. In 2003, there was an outbreak of SARS in China that spread to other countries and then ended in 2004. SARS-CoV-2 has spread faster than the 2003 SARS. SARS-CoV-2 is spread when an infected person coughs or sneezes droplets of saliva or mucus with the virus into the air. The respiratory droplets usually do not go further than a few feet, are airbourne for a few moments, and then land on a surface. SARS-CoV-2 has an incubation period of 2 to 14 days and the symptoms of the virus include cough, fever or chills, shortness of breath or difficulty breathing, muscle or body aches, sore throat, loss of taste or smell, diarrhea, headache, fatigue, nausea or vomiting, congestion or runny nose, and in rare cases the virus can lead to difficulty walking, confusion, bluish face or lips, coughing up blood, severe respiratory problems, kidney failure, high fever, or death. The following is a diagram of the symptoms.
![image](https://user-images.githubusercontent.com/56414953/112048677-0b072300-8b25-11eb-8840-d80b978cf20b.png)
# SARS-CoV-2 Biology
Coronaviruses are a sphere-like 20-sided polygon, icosahedron, shape and belong to the Nidovirales order. SARS-CoV-2 travels through the respitory tract and attaches itself to alveoli, air sacs, in the lungs. Coronaviruses are named after the dyed red spike glycoproteins (S) that cover them and attach these protiens by being activated by the host cell's proteases, ACE2 and TMPRSS2 ennzymes, at a sequential proteolytic cleavage S1 and S2 site to fuse with a host cell's enzymes to enter, endocytosis, the cell's plasma membrane to the cytosol. S1 is the end binding region of the S protein and S2 is the beam of the S protien. The spike glcoproteins can also attach to a cell's endosomes being activated by the host cell's CTSL enzyme. Inside of the icosahedron positive-sensed lipid bilayer envelope is a helical capsid (N) that encloses a nucleic acid genome, which encodes the viral genetic information -- non-segmented-single-stranded RNA -- that is used during the lytic cycle to generate RNA polymerase, protease, and other proteins. The virus leaves the capsid ouside of the cell when performing endocytosis. The DNA template of the host cell is transcribed by helicase enzyme separating the two nucleic acid strands of the DNA, the DNA polymerase enzyme catalyzes the synthesis of RNA molecules -- adenine (A) to uracil (U), thymine (T) to adenine (A), guanine (G) to cytosine (C), and cytosine (C) to guanine (G)-- and the DNA ligase enzyme joins the strands to make multiple genomic and subgenomic viral mRNA. The mRNA is then translated with ribosomes using tRNA that attaches anticodons to the mRNA codons in the Rough Endoplasmic Reticulum to build viral amino acid molecules that form a viral protien chain of polypeptides that are further assembled in the Golgi Aparatus and then stored in vesicles. The dyed yellow envelope proteins (E) and dyed orange membrane glycoproteins (M) assist in budding -- using the host cell's plasma membrane for envelope formation -- and then exiting, exocytosis, the host cell through lysis. The following is a diagram of the SARS-CoV-2 lifecycle.
![image](https://user-images.githubusercontent.com/56414953/112049490-14dd5600-8b26-11eb-9c3c-5ed65b39cc46.png)
ACE2 modulates the activity of the angiotensin II protein, which increases blood pressure and inflammation. The SARS-CoV-2 virus binding to ACE2 inhibits ACE2 and can cause an increase in cell inflammation resulting in the death of cells in the alveoli units with hypoxic fluid flooding, an increase in blood preasure damaging blood vessels causing microvascular thrombosis, and the tranduction of the kidney podocytes resulting in acute kidney injury. The following is a diagram of the enzymes that get inhibited and the parts of the body that can get damaged.
![image](https://user-images.githubusercontent.com/56414953/112049125-98e30e00-8b25-11eb-95b7-f4a19ebf0a77.png)
# Testing for SARS-CoV-2
A patient can be tested for SARS-CoV-2 with the sequence-specific molecular nucleic acid assay, or the antigen-specific immunoassay. For a molecular-assay, a nasal or saliva sample is collected from upper respiratory fluid and then Real-time RT-PCR is conducted to quantify sequences within the RNA samples. Reverse transcriptase converts extracted RNA into cDNA that is used as a template for DNA polymerase to complete the strand of dsDNA and then RT-PCR amplifies the genetic regions and fluorescent probes bind to the regions for identification. For an immuno-assay, antibodies are put on a membrane and complexed with a potentialy virulent sample of which any antigen will be trapped that results in the membrane changing color. A SARS-CoV-2 recovered patient can be tested for whether the patient has developed anibodies against the virus by checking a blood sample for the antibodies. The following are diagrams of a molecular assay

![image](https://user-images.githubusercontent.com/56414953/112049170-a6989380-8b25-11eb-8d39-89612a07e920.png)

and an immuno assay.
![image](https://user-images.githubusercontent.com/56414953/112049200-aef0ce80-8b25-11eb-8301-43ff58f546ce.png)
# Vaccines for SARS-CoV-2
Vaccines have been developed to combat SARS-CoV-2. The Pfizer/BioNTech vaccine (BNT162b2) and The ModernaTX, Inc vaccine (mRNA-1273) are mRNA vaccines. mRNA vaccines deliver lab designed viral mRNA made by coding both the 5’-untranslated region (UTR) and the 3’-UTR into cells where it is translated into the encoded antigen to which an immune recognition by white blood cells, immunogenicity, results. The AstraZeneca in collaboration with the University of Oxford vaccine (AZD1222) is an adenovirus vaccine. Adenovirus vaccines are first gene sub-cloned into an intermediary vector, transfered to an adenovirus recombinant genome vector, transfected into packaging cells, amplified into a culture stock, and then titrated to determine the concentration of active adenoviruses in the stock. The adenoviruse is then delivered to cells where immunogenicity results. The following is a diagram of Virus vector DNA and mRNA vaccine immune response production.
Vaccines have been developed to combat SARS-CoV-2. The Pfizer/BioNTech vaccine (BNT162b2) and The ModernaTX, Inc vaccine (mRNA-1273) are mRNA vaccines. mRNA vaccines deliver lab designed viral mRNA made by coding both the 5’-untranslated region (UTR) and the 3’-UTR into cells where it is translated into the encoded antigen to which an immune recognition by white blood cells, immunogenicity, results. The AstraZeneca in collaboration with the University of Oxford vaccine (AZD1222) is an adenovirus vaccine. Adenovirus vaccines are first gene sub-cloned into an intermediary vector, transfered to an adenovirus recombinant genome vector, transfected into packaging cells, amplified into a culture stock, and then titrated to determine the concentration of active adenoviruses in the stock. The adenoviruse is then delivered to cells where immunogenicity results. The following is a diagram of Virus vector DNA and mRNA vaccine immune response production.
![image](https://user-images.githubusercontent.com/56414953/112049237-badc9080-8b25-11eb-9a75-617ebe526286.png)
# Covid-19 Totals
22% of the global population has been tested for the virus. 6.9% of the tested global population has been diagnosed with the virus. 80.6% of global cases have recovered and 2.2% have died from the virus. 5.1% of the global population has been vaccinated.  The United States has the most cases of the virus and it is likely because it has tested more than other countries.
![image](https://user-images.githubusercontent.com/56414953/112051811-c2516900-8b28-11eb-888c-feda788c0de7.png)
![image](https://user-images.githubusercontent.com/56414953/112051843-caa9a400-8b28-11eb-8950-cb8b9805702a.png)
![image](https://user-images.githubusercontent.com/56414953/112051957-e8770900-8b28-11eb-8be7-3a388b1b81eb.png)
![image](https://user-images.githubusercontent.com/56414953/112051995-f2007100-8b28-11eb-9097-8a8a05bf1d0f.png)
![image](https://user-images.githubusercontent.com/56414953/112052024-fa58ac00-8b28-11eb-8825-de14b496a142.png)
![image](https://user-images.githubusercontent.com/56414953/112052042-00e72380-8b29-11eb-8f8d-1ce4cfe08ee0.png)
![image](https://user-images.githubusercontent.com/56414953/112052052-06dd0480-8b29-11eb-94f9-a87d0106deb1.png)
![image](https://user-images.githubusercontent.com/56414953/112052076-0d6b7c00-8b29-11eb-9afc-852e372e4f1c.png)
![image](https://user-images.githubusercontent.com/56414953/112052122-2116e280-8b29-11eb-9e72-bc802007c56d.png)
![image](https://user-images.githubusercontent.com/56414953/112052147-2b38e100-8b29-11eb-81ef-8c5b26d1127c.png)
![image](https://user-images.githubusercontent.com/56414953/112052203-3c81ed80-8b29-11eb-885b-55490471f7e9.png)
![image](https://user-images.githubusercontent.com/56414953/112052235-460b5580-8b29-11eb-90f7-ee1149d48f74.png)
![image](https://user-images.githubusercontent.com/56414953/112052264-4d326380-8b29-11eb-8723-d583f48fafb8.png)
![image](https://user-images.githubusercontent.com/56414953/112052288-53284480-8b29-11eb-808a-8f795b998abf.png)
![image](https://user-images.githubusercontent.com/56414953/112052308-59b6bc00-8b29-11eb-89eb-a45fcbe81394.png)
![image](https://user-images.githubusercontent.com/56414953/112052331-60ddca00-8b29-11eb-84c2-9e5f01fcd0f6.png)
![image](https://user-images.githubusercontent.com/56414953/112052346-66d3ab00-8b29-11eb-91c7-17f00715b260.png)
![image](https://user-images.githubusercontent.com/56414953/112052375-6cc98c00-8b29-11eb-9b09-8e5c285f5ad3.png)
![image](https://user-images.githubusercontent.com/56414953/112052386-73580380-8b29-11eb-9849-0d4a4ab28c3b.png)
![image](https://user-images.githubusercontent.com/56414953/112052406-794de480-8b29-11eb-894c-900bd183ce19.png)
![image](https://user-images.githubusercontent.com/56414953/112052429-81a61f80-8b29-11eb-8c7e-72e2375bef96.png)
![image](https://user-images.githubusercontent.com/56414953/112052502-94b8ef80-8b29-11eb-8d16-e651382ac4d5.png)
![image](https://user-images.githubusercontent.com/56414953/112052527-9da9c100-8b29-11eb-8781-f4ae753cb1b0.png)
![image](https://user-images.githubusercontent.com/56414953/112052560-a4383880-8b29-11eb-8742-66338eeaf82a.png)

# Government Regulation Features
The Governments' responses to COVID19 are the measures implemented by governments worldwide in response to the Coronavirus pandemic. There are two types of measures: public health measures and economic measures.
The variables are :

- cases: binary variable equal to 1 if there were cases of SARS-CoV-2 and 0 otherwise;
- school: binary variable equal to 1 if schools were closed and 0 otherwise;
- domestic: binary variable equal to 1 if there was a domestic lockdown and 0 otherwise;
- travel: binary variable equal to 1 if travel restrictions were implemented and 0 otherwise;
- travel_dom: binary variable equal to 1 if travel restrictions within the country (e.g. inter-region travels) were implemented and 0 otherwise;
- curf: binary variable equal to 1 if a curfew was implemented and 0 otherwise;
- mass: binary variable equal to 1 if bans on mass gatherings were implemented and 0 otherwise;
- elect: binary variable equal to 1 if some elections were postponed and 0 otherwise;
- sport: binary variable equal to 1 if bans on sporting and large events were implemented and 0 otherwise;
- rest: binary variable equal to 1 if restaurants were closed and 0 otherwise;
- testing: binary variable equal to 1 if there was a public testing policy and 0 otherwise;
- surveillance: binary variable equal to 1 if mobile app or bracelet surveillance was implemented and 0 otherwise;
- masks binary variable equal to 1 if the obligationsto wear masks in public spaces was implemented and 0 otherwise;
- state: binary variable equal to 1 if the state of emergency is declared and 0 otherwise;
- cash: binary variable equal to 1 if cash transfers are implemented and 0 otherwise;
- wage: binary variable equal to 1 if wage support is implemented and 0 otherwise;
- credit: binary variable equal to1 if credit schemes are implemented and 0 otherwise;
- taxc: binary variable equal to 1 if tax credits are implemented and 0 otherwise;
- taxd: binary variable equal to 1 if tax delays are implemented and 0 otherwise;
- export: binary variable equal to 1 if supports to importers or exporters are implemented and 0 otherwise;
- rate: binary variable equal to 1 if the Central Bank lowered the interest rates and 0 otherwise;
# Conclusion
The time-series models suggest that vaccinations will trend upward by 245% and cases of the virus will trend downward by 54%. The logit model suggests that the government regulations of school closures, travel restrictions, state of emergency declarations, wage support, tax credits, and interest rate lowering decreased the log odds of the presence of virus cases. Government regulations such as disallowing public gatherings and mandating wearing masks did not decrease the log odds of the presence of virus cases. The virus travels in sneezed or coughed droplets of mucus or saliva, is airborne for a few moments, and then lands on a surface. Instead of wearing masks and preventing gatherings, carrying a handkerchiefs in which people could sneeze or cough and sanitizing areas were people gather would be sufficient in preventing the spread of SARS-CoV-2.
