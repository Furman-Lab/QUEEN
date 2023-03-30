# QUEEN_prediction
QUEEN_prediction
all_model_data column explanantion:
nsub: assigned qs from qsbio (nsub=number of subunits)
1	2	3	4	5	6	7	8	10	12	14	24: columns representing the prediction probability to each qs class 
code: pdb code with underscore of the serial number of qsbio for this complex
representative: used for clustering for separation of train/test sets. Determined by MMseqs	
1_pred	2_pred	3_pred: The highest, second and third prediction (based on the prediction probabilities above)
top_2:prediction based on the top 2 (1_pred, 2_pred) predictions
pdb: pdb code without the qsbio complex numbering
#uid: ecod internal domain unique identifier
ecod_domain_id: domain identifier
manual_rep: ECOD representative status - manual (curated) or automated nonrep
f_id: ECOD hierachy identifier - [X-group].[H-group].[T-group].[F-group]
chain: Chain identifier (note: case-sensitive)
pdb_range: PDB residue number range
seqid_range: seq_id number range (based on internal PDB indices)
unp_acc: uniprot accesion
arch_name	x_name	h_name	t_name	f_name:	name of corresponding hierachies
asm_status: Domain assembly status (if domain is member of assembly, partners' ecod domain ids listed)
seq_length: calculated for the range, longest segment was chosen for entries with more than 1 domain
set: set to which the entry belongs (train_set, holdout_set)
