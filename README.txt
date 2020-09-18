To make the script executable use command:
chmod +x <scriptname>


script_biom_to_txt_dir converts .biomfiles to tsv format in the given directory
clear_script clears .csv tables in the directory
script_txt_to_ofg_csv splits the whole directory files from a txt table to 3 csv tables with the taxonomy information on the levels o, f and g. It interprets the missing taxonomy data as marked by empty (o__, s__, etc.)
for_script notebook contains the notebook code for the splitting of a single tabular txt data item. It is then converted to the python code by  the script_txt_to_ofg_csv
