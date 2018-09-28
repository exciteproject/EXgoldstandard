# Gold Standard Data for Matching Algorithm

This gold standard is created for the evaluation and training of the [citation matching](https://github.com/exciteproject/ref_matcher) algorithm in the [EXCITE](http://excite.west.uni-koblenz.de/website/) project.

## Reference strings set in the gold standard

This collection of data was created by following these steps:
  1. [One of EXCITE reference strings extraction algorithms]( https://github.com/exciteproject/refext) was applied on our PDF corpora, and the result of this phase was a collection of reference strings. These references may contain some errors inside since they were extracted automatically (without any human support to correct them). 
  2. Afterward, some of these reference strings were selected randomly for the next step.
  3. Then the EXCITE reference segmentation algorithm was applied on the set of references of step 2.
  4. In the final stage, a human assessor created the list of all matches (in [Sowiport](http://sowiport.gesis.org/)) for each reference string.
  
The results of these steps were stored in [DataSet_A csv](https://raw.githubusercontent.com/exciteproject/GoldStandard_for_matching/master/Datasets_for_matching/%5BDataSet_A%5D_Extracted_references_and_Match_IDs.csv) file. This CSV file contains 816 reference strings with 4 columns:

  1. ref_id,
  2. reference_strings,
  3. reference_segementations,
  4. Math_ids_in_sowiport. 

Out of all references in the set, 521 items have at least one match item in sowiport.


## Target set in the gold standard for matching of reference strings against

Sowiport contained more than 9 million bibliographic records. We publish a smaller set of data from sowiport that allows experiments with the Gold standard.  

This set of data was stored as [DataSet_B](https://raw.githubusercontent.com/exciteproject/GoldStandard_for_matching/master/Datasets_for_matching/%5BDataSet_B%5D_samll_collection_data_in_sowiport.csv) csv file. This set of data includes 18,590 bibliographic items and 16 columns:

  1. 'id': sowiport id ,
  2. 'title_full': the full title of the article,
  3. 'title_sub': the sub title of the article,
  4. 'facet_person_str_mv': authors' names used for facet in sowiport ,
  5. 'person_author_normalized_str_mv': normalized format of authors' family names,
  6. 'journal_short_txt_mv': short title format of journal,
  7. 'journal_title_txt_mv': the full title of journal,
  8. 'norm_pagerange_str': normalize format of page information,
  9. 'norm_publishDate_str': normalized publish year infromation,
  10. 'norm_title_full_str': normalized format of full title,
  11. 'norm_title_str': normalized format of sub title,
  12. 'norm_volume_str': normalized format of volume information,
  13. 'norm_issue_str': normalized format of issue information,
  14. 'recorddoi_str_mv': doi information,
  15. 'zsabk_str': abbrivation of journal title,
  16. 'db_origin_str': source of the information in Sowiport.
