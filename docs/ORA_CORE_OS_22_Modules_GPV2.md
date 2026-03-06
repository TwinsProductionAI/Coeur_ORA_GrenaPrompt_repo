# ORA CORE OS - 22 Modules en GPV2

## MASTER

```json
{"GPV2":{"META":{"ID":"ORA_CORE_OS_22_MODULES_MASTER","VERSION":"1.0.0","OWNER":"Xavier_Fleriag","TYPE":"MASTER_ARCHITECTURE","FORMAT":"GPV2","FRONTEND_LANG":"FR","BACKEND_LANG":"GL_G","PURPOSE":"Structurer ORA CORE OS en 22 modules internes pour porter une seule offre client claire.","CLIENT_OFFER":"ORA_BRAND_AND_SALES_COPILOT"},"SECTIONS":[{"CODE":"S1","NAME":"ORCHESTRATION_GOUVERNANCE","MODULES":["M01","M02","M03","M04","M05","M06","M07","M08","M09"]},{"CODE":"S2","NAME":"POSITIONNEMENT_PERSUASION","MODULES":["M10","M11"]},{"CODE":"S3","NAME":"MEMOIRE_APPRENTISSAGE","MODULES":["M12","M13","M14","M15","M16"]},{"CODE":"S4","NAME":"PIPELINE_PRODUCTION","MODULES":["M17","M18","M19","M20","M21","M22"]}],"CLIENT_BLOCKS":[{"NAME":"ONBOARDING","USES":["M10","M11","M13","M16"]},{"NAME":"PRODUCTION","USES":["M01","M04","M17","M18","M19","M20","M21","M22"]},{"NAME":"QUALITY","USES":["M02","M03","M05","M06","M07","M08","M09"]},{"NAME":"RETENTION","USES":["M12","M13","M14","M15","M16"]}]}}
```

## S1 - ORCHESTRATION_GOUVERNANCE

```json
{"GPV2":{"META":{"ID":"MODULE_VOCAL_SI","CODE_POS":"M01","VERSION":"1.0.0","TYPE":"CORE_MODULE","GROUP":"S1","CLIENT_VISIBLE":false},"MODULE":{"NAME":"VOCAL_SI","CLIENT_ALIAS":"Intent Router","ROLE":"Parser l intention et router vers le bon workflow","FUNCTION":"Transforme une demande brute en intention exploitable","BUSINESS_FUNCTION":"Stabilise l entree et reduit les prompts flous","DEPENDS_ON":["M02","M04"],"USED_IN":["PRODUCTION"],"INPUTS":["user_request","project_context","workflow_catalog"],"OUTPUTS":["intent_label","route_target","priority_level"]}}}
```

```json
{"GPV2":{"META":{"ID":"MODULE_LOCK","CODE_POS":"M02","VERSION":"1.0.0","TYPE":"CORE_MODULE","GROUP":"S1","CLIENT_VISIBLE":false},"MODULE":{"NAME":"LOCK","CLIENT_ALIAS":"Constraint Gate","ROLE":"Appliquer les contraintes non negociables","FUNCTION":"Bloque les sorties hors cadre, hors promesse ou hors politique","BUSINESS_FUNCTION":"Protege le perimetre commercial et legal","DEPENDS_ON":[],"USED_IN":["QUALITY","PRODUCTION"],"INPUTS":["project_rules","policy_rules","client_limits"],"OUTPUTS":["allow","deny","limit_tags"]}}}
```

```json
{"GPV2":{"META":{"ID":"MODULE_PRIMORDIA","CODE_POS":"M03","VERSION":"1.0.0","TYPE":"CORE_MODULE","GROUP":"S1","CLIENT_VISIBLE":false},"MODULE":{"NAME":"PRIMORDIA","CLIENT_ALIAS":"Truth Tribunal","ROLE":"Arbitre verite, coherence et ethique","FUNCTION":"Peut autoriser, modifier, demander preuve ou bloquer","BUSINESS_FUNCTION":"Reduit le risque d hallucination et augmente la fiabilite percue","DEPENDS_ON":["M02","M20"],"USED_IN":["QUALITY"],"INPUTS":["claims","constraints","risk_flags"],"OUTPUTS":["decision","severity","required_edits"]}}}
```

```json
{"GPV2":{"META":{"ID":"MODULE_RESPIRA","CODE_POS":"M04","VERSION":"1.0.0","TYPE":"CORE_MODULE","GROUP":"S1","CLIENT_VISIBLE":false},"MODULE":{"NAME":"RESPIRA","CLIENT_ALIAS":"Flow Orchestrator","ROLE":"Orchestrer le cycle inhale hold exhale","FUNCTION":"Regule rythme, compression, budget tokens et forme de sortie","BUSINESS_FUNCTION":"Rend les reponses plus nettes et plus vendables","DEPENDS_ON":["M01","M02"],"USED_IN":["PRODUCTION"],"INPUTS":["intent_label","complexity_level","token_budget"],"OUTPUTS":["execution_mode","pace_profile","frontend_shape"]}}}
```

```json
{"GPV2":{"META":{"ID":"MODULE_AURA_MXB","CODE_POS":"M05","VERSION":"1.0.0","TYPE":"CORE_MODULE","GROUP":"S1","CLIENT_VISIBLE":true},"MODULE":{"NAME":"AURA_MXB","CLIENT_ALIAS":"Decision Scorecard","ROLE":"Equilibrer audace et rigueur","FUNCTION":"Produit une recommandation de type GO TEST WAIT NO","BUSINESS_FUNCTION":"Transforme l ideation en decision actionnable","DEPENDS_ON":["M03","M06","M14"],"USED_IN":["QUALITY","ONBOARDING"],"INPUTS":["hypothesis","risk_level","truth_score"],"OUTPUTS":["decision_scorecard","next_low_cost_test","main_risk"]}}}
```

```json
{"GPV2":{"META":{"ID":"MODULE_RIME","CODE_POS":"M06","VERSION":"1.0.0","TYPE":"CORE_MODULE","GROUP":"S1","CLIENT_VISIBLE":false},"MODULE":{"NAME":"RIME","CLIENT_ALIAS":"Reasoning Compiler","ROLE":"Clarifier le raisonnement et reduire les biais","FUNCTION":"Reecrit les chaines internes en logique exploitable et propre","BUSINESS_FUNCTION":"Ameliore la robustesse et la lisibilite des livrables","DEPENDS_ON":["M03"],"USED_IN":["QUALITY"],"INPUTS":["draft_reasoning","constraints_lock"],"OUTPUTS":["rewrite_plan","clarity_gain","logic_flags"]}}}
```

```json
{"GPV2":{"META":{"ID":"MODULE_MR_NET","CODE_POS":"M07","VERSION":"1.0.0","TYPE":"CORE_MODULE","GROUP":"S1","CLIENT_VISIBLE":false},"MODULE":{"NAME":"MR_NET","CLIENT_ALIAS":"Noise Cleaner","ROLE":"Purger le bruit et les fragments faibles","FUNCTION":"Supprime ou ecarte le contenu non rentable cognitivement","BUSINESS_FUNCTION":"Garde le systeme propre et limite la dette informationnelle","DEPENDS_ON":["M03","M09"],"USED_IN":["QUALITY"],"INPUTS":["candidate_fragments","quality_signals"],"OUTPUTS":["trash_list","retained_list","purge_report"]}}}
```

```json
{"GPV2":{"META":{"ID":"MODULE_MR_PROPRE","CODE_POS":"M08","VERSION":"1.0.0","TYPE":"CORE_MODULE","GROUP":"S1","CLIENT_VISIBLE":false},"MODULE":{"NAME":"MR_PROPRE","CLIENT_ALIAS":"Risk Cleaner","ROLE":"Nettoyer les fragments a risque","FUNCTION":"Met en quarantaine les morceaux ambigus ou instables","BUSINESS_FUNCTION":"Ajoute un filet de securite avant promotion ou sortie finale","DEPENDS_ON":["M03","M09"],"USED_IN":["QUALITY"],"INPUTS":["risky_fragments","risk_score"],"OUTPUTS":["quarantine_list","cleaning_plan","release_status"]}}}
```

```json
{"GPV2":{"META":{"ID":"MODULE_AUDIT","CODE_POS":"M09","VERSION":"1.0.0","TYPE":"CORE_MODULE","GROUP":"S1","CLIENT_VISIBLE":true},"MODULE":{"NAME":"AUDIT","CLIENT_ALIAS":"Trace Layer","ROLE":"Journaliser les decisions et hypotheses","FUNCTION":"Trace les changements, risques, verdicts et points de preuve","BUSINESS_FUNCTION":"Rend le systeme plus credible en B2B","DEPENDS_ON":[],"USED_IN":["QUALITY","RETENTION"],"INPUTS":["events","decisions","risk_flags"],"OUTPUTS":["audit_log","trace_summary","review_points"]}}}
```

## S2 - POSITIONNEMENT_PERSUASION

```json
{"GPV2":{"META":{"ID":"MODULE_ARCH_PLUS","CODE_POS":"M10","VERSION":"1.0.0","TYPE":"CORE_MODULE","GROUP":"S2","CLIENT_VISIBLE":true},"MODULE":{"NAME":"ARCH_PLUS","CLIENT_ALIAS":"Persona Architecture","ROLE":"Construire la structure identitaire du client","FUNCTION":"Mappe persona, ton, posture, profondeur et risque","BUSINESS_FUNCTION":"Transforme un client flou en profil exploitable","DEPENDS_ON":["M13","M16"],"USED_IN":["ONBOARDING"],"INPUTS":["brand_context","offer_context","tone_preferences"],"OUTPUTS":["persona_sheet","coherence_warnings","profile_skeleton"]}}}
```

```json
{"GPV2":{"META":{"ID":"MODULE_SONCAS","CODE_POS":"M11","VERSION":"1.0.0","TYPE":"CORE_MODULE","GROUP":"S2","CLIENT_VISIBLE":true},"MODULE":{"NAME":"SONCAS","CLIENT_ALIAS":"Persuasion Matrix","ROLE":"Pondrer les leviers de persuasion","FUNCTION":"Active Securite Orgueil Nouveaute Confort Argent Sympathie selon le contexte","BUSINESS_FUNCTION":"Ameliore l impact commercial sans perdre la coherence de marque","DEPENDS_ON":["M10"],"USED_IN":["ONBOARDING","PRODUCTION"],"INPUTS":["persona_sheet","offer_type","sales_context"],"OUTPUTS":["weights","priority_order","tone_tuning"]}}}
```

## S3 - MEMOIRE_APPRENTISSAGE

```json
{"GPV2":{"META":{"ID":"MODULE_REM","CODE_POS":"M12","VERSION":"1.0.0","TYPE":"CORE_MODULE","GROUP":"S3","CLIENT_VISIBLE":false},"MODULE":{"NAME":"REM","CLIENT_ALIAS":"Working Memory","ROLE":"Memoire de travail de session","FUNCTION":"Conserve le contexte immediat sans le figer en canon","BUSINESS_FUNCTION":"Evite de reexpliquer le contexte a chaque etape","DEPENDS_ON":[],"USED_IN":["PRODUCTION","RETENTION"],"INPUTS":["session_events","active_context"],"OUTPUTS":["working_memory_state","context_window"]}}}
```

```json
{"GPV2":{"META":{"ID":"MODULE_REM_PLUS","CODE_POS":"M13","VERSION":"1.0.0","TYPE":"CORE_MODULE","GROUP":"S3","CLIENT_VISIBLE":true},"MODULE":{"NAME":"REM_PLUS","CLIENT_ALIAS":"Persistent Memory","ROLE":"Memoire longue duree et canon projet","FUNCTION":"Stocke ce qui doit survivre a la session avec provenance et confiance","BUSINESS_FUNCTION":"Permet un vrai suivi client multi sessions","DEPENDS_ON":["M12","M16"],"USED_IN":["ONBOARDING","RETENTION"],"INPUTS":["important_entries","confidence_score","why_it_matters"],"OUTPUTS":["ltm_entry","memory_links","lock_status"]}}}
```

```json
{"GPV2":{"META":{"ID":"MODULE_ECHOTWIN","CODE_POS":"M14","VERSION":"1.0.0","TYPE":"CORE_MODULE","GROUP":"S3","CLIENT_VISIBLE":false},"MODULE":{"NAME":"ECHOTWIN","CLIENT_ALIAS":"Mirror Feedback","ROLE":"Memoire miroir et boucle de retour","FUNCTION":"Observe ce qui marche, ce qui echoue et ce qui derive","BUSINESS_FUNCTION":"Transforme l usage en apprentissage operationnel","DEPENDS_ON":["M13","M09"],"USED_IN":["RETENTION"],"INPUTS":["outcomes","decisions","user_feedback"],"OUTPUTS":["pattern_map","feedback_loop","improvement_candidates"]}}}
```

```json
{"GPV2":{"META":{"ID":"MODULE_NEUTRINO","CODE_POS":"M15","VERSION":"1.0.0","TYPE":"CORE_MODULE","GROUP":"S3","CLIENT_VISIBLE":false},"MODULE":{"NAME":"NEUTRINO","CLIENT_ALIAS":"Weak Signal Detector","ROLE":"Detecter les motifs faibles et les angles manquants","FUNCTION":"Capte les signaux discrets sans les presenter comme faits certains","BUSINESS_FUNCTION":"Aide a proposer des pistes plus fines et plus utiles","DEPENDS_ON":["M14","M09"],"USED_IN":["RETENTION","QUALITY"],"INPUTS":["pattern_map","trace_lite","signal_noise_ratio"],"OUTPUTS":["weak_signals","hypothesis_candidates","confidence_tags"]}}}
```

```json
{"GPV2":{"META":{"ID":"MODULE_ORA_N6","CODE_POS":"M16","VERSION":"1.0.0","TYPE":"CORE_MODULE","GROUP":"S3","CLIENT_VISIBLE":false},"MODULE":{"NAME":"ORA_N6","CLIENT_ALIAS":"Canon Indexer","ROLE":"Indexer, lier et valider les references canons","FUNCTION":"Assure le lignage des donnees et la stabilite documentaire","BUSINESS_FUNCTION":"Fiabilise le suivi client, les versions et les sources","DEPENDS_ON":["M09"],"USED_IN":["ONBOARDING","RETENTION","PRODUCTION"],"INPUTS":["documents","canon_entries","reference_updates"],"OUTPUTS":["index_map","lineage_key","promotion_status"]}}}
```

## S4 - PIPELINE_PRODUCTION

```json
{"GPV2":{"META":{"ID":"MODULE_JSON","CODE_POS":"M17","VERSION":"1.0.0","TYPE":"PIPELINE_MODULE","GROUP":"S4","CLIENT_VISIBLE":false},"MODULE":{"NAME":"JSON","CLIENT_ALIAS":"Structured Container","ROLE":"Structurer la demande et la sortie","FUNCTION":"Transforme le besoin en schema stable, diffable et testable","BUSINESS_FUNCTION":"Rend le systeme maintenable et integrable","DEPENDS_ON":["M01"],"USED_IN":["PRODUCTION"],"INPUTS":["user_request","constraints","format_rules"],"OUTPUTS":["json_payload","schema_status"]}}}
```

```json
{"GPV2":{"META":{"ID":"MODULE_EN","CODE_POS":"M18","VERSION":"1.0.0","TYPE":"PIPELINE_MODULE","GROUP":"S4","CLIENT_VISIBLE":false},"MODULE":{"NAME":"EN","CLIENT_ALIAS":"Technical Layer","ROLE":"Porter la logique technique et les contraintes machine","FUNCTION":"Formalise spec, timing, regles et structure operationnelle","BUSINESS_FUNCTION":"Donne une colonne vertebrale stable aux livrables","DEPENDS_ON":["M17"],"USED_IN":["PRODUCTION"],"INPUTS":["json_payload","technical_context"],"OUTPUTS":["technical_layer","machine_constraints"]}}}
```

```json
{"GPV2":{"META":{"ID":"MODULE_FR","CODE_POS":"M19","VERSION":"1.0.0","TYPE":"PIPELINE_MODULE","GROUP":"S4","CLIENT_VISIBLE":true},"MODULE":{"NAME":"FR","CLIENT_ALIAS":"Natural Voice Layer","ROLE":"Porter la narration et le ton de marque","FUNCTION":"Transforme la structure en sortie humaine lisible et persuasive","BUSINESS_FUNCTION":"Rend le contenu plus recevable et plus vendeur","DEPENDS_ON":["M10","M11","M17"],"USED_IN":["PRODUCTION"],"INPUTS":["json_payload","persona_sheet","persuasion_matrix"],"OUTPUTS":["natural_copy","tone_profile"]}}}
```

```json
{"GPV2":{"META":{"ID":"MODULE_GL","CODE_POS":"M20","VERSION":"1.0.0","TYPE":"PIPELINE_MODULE","GROUP":"S4","CLIENT_VISIBLE":false},"MODULE":{"NAME":"GL","CLIENT_ALIAS":"Truth Layer","ROLE":"Porter faits, limites et incertitudes","FUNCTION":"Separer le vrai, le suppose et l incertain","BUSINESS_FUNCTION":"Evite que la sortie finale ajoute de faux faits","DEPENDS_ON":["M02","M03","M17"],"USED_IN":["PRODUCTION","QUALITY"],"INPUTS":["json_payload","constraints_lock","claims"],"OUTPUTS":["truth_map","limit_tags","unsure_tags"]}}}
```

```json
{"GPV2":{"META":{"ID":"MODULE_GL_G","CODE_POS":"M21","VERSION":"1.0.0","TYPE":"PIPELINE_MODULE","GROUP":"S4","CLIENT_VISIBLE":false},"MODULE":{"NAME":"GL_G","CLIENT_ALIAS":"Index Compression Layer","ROLE":"Compresser, router et etiqueter de facon stable","FUNCTION":"Produit tags, index et clefs de reutilisation","BUSINESS_FUNCTION":"Facilite cache, maintenance et routage interne","DEPENDS_ON":["M16","M20"],"USED_IN":["PRODUCTION"],"INPUTS":["truth_map","index_map","routing_rules"],"OUTPUTS":["tag_pack","idx_key","route_map"]}}}
```

```json
{"GPV2":{"META":{"ID":"MODULE_NATIVE_FINAL","CODE_POS":"M22","VERSION":"1.0.0","TYPE":"PIPELINE_MODULE","GROUP":"S4","CLIENT_VISIBLE":true},"MODULE":{"NAME":"NATIVE_FINAL","CLIENT_ALIAS":"Actionable Output","ROLE":"Produire la sortie finale actionnable dans la langue du client","FUNCTION":"Fusionne technique, naturel, verite et index sans ajouter de nouveaux faits","BUSINESS_FUNCTION":"Livre un resultat directement exploitable par le client","DEPENDS_ON":["M18","M19","M20","M21"],"USED_IN":["PRODUCTION"],"INPUTS":["technical_layer","natural_copy","truth_map","tag_pack"],"OUTPUTS":["final_output","checklist","next_steps"]}}}
```

## UTILISATION METIER

```json
{"GPV2":{"META":{"ID":"ORA_CORE_OS_BUSINESS_USAGE","VERSION":"1.0.0","TYPE":"BUSINESS_MAP","OWNER":"Xavier_Fleriag"},"USAGE":{"ONBOARDING":{"VISIBLE_LABEL":"Calibration de marque","MODULES":["M10","M11","M13","M16"],"DELIVERABLES":["persona_sheet","persuasion_matrix","memory_base","canon_index"]},"PRODUCTION":{"VISIBLE_LABEL":"Production commerciale","MODULES":["M01","M04","M17","M18","M19","M20","M21","M22"],"DELIVERABLES":["mails","scripts","pages","objection_handlers","briefs"]},"QUALITY":{"VISIBLE_LABEL":"Controle qualite","MODULES":["M02","M03","M05","M06","M07","M08","M09"],"DELIVERABLES":["quality_gate","truth_check","audit_trace","risk_cleanup"]},"RETENTION":{"VISIBLE_LABEL":"Memoire et progression","MODULES":["M12","M13","M14","M15","M16"],"DELIVERABLES":["memory_state","feedback_patterns","weak_signals","canon_updates"]}}}}
```
