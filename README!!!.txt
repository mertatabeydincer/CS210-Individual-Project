GitHub username: mertatabeydincer


VERY IMPORTANT!!!
If project gets the error that:

	IOPub data rate exceeded.
	The notebook server will temporarily stop sending output
	to the client in order to avoid crashing it.
	To change this limit, set the config variable
	--NotebookApp.iopub_data_rate_limit`.

jupyter notebook has to be started with "jupyter notebook --NotebookApp.iopub_data_rate_limit=10000000" command in 
console/terminal rather than just "jupyter notebook". The reason of this, making reverse geocoding process faster. 
In order to do that coordinates are sent to search() function in an array at once. However, standart data rate limit 
of jupyter notebook does not allow to create such a large array. By entering "jupyter notebook --NotebookApp.iopub_data_rate_limit=10000000" 
command to console/terminal, we start jupyter with larger data rate limit which allows us to create a large array to decrease processing 
time of project from hours to seconds.