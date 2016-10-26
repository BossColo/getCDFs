# getCDFs
This will check for cdfs on your computer. If they don't exist, or there's an updated version on the server, it will download from the server. It will then load the cdfs using spacepy.pycdf, and place them into a dictionary.

##Usage:
getCDFs(getCDFs(datetime, craft, species, PH='LEHT', EMF='1sec-sm', all=True, TOFxE=False, TOFxPH=False, HOPE=False, EMFISIS=False):

datetime is a Python datetime object, craft is a character: 'A' or 'B', species is a character: 'H', 'He', or 'O', PH is a string describing which Time of Flight by Pulse Height product you want: 'LEHT'(Low Energy, High Time resolution) or 'HELT'(High Energy, Low Time resolution), EMF is a string describing which EMFISIS product you want: ('1sec', '4sec', or 'hires')+'-'+('gei', 'geo', 'gse', 'gsm', or 'sm'). The last five keywords describe which data product you want, all is default, but if you set any one or more of them to True, then you will only get what you set to True.

changeRoot()

On the first run, you will be asked to set a root directory where your files will be stored. This function will allow you to change this.
