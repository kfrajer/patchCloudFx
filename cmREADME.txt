gcloud auth login 
gcloud app deploy -v adv-patch-cf
gcloud app deploy -v patch-cf 

python -m virtualenv env 
env\Scripts\activate 
python -m pip install -r requirements.txt
deactivate

TEST ENDPOINT: http://patch-cf-dot-wp-phpso2-8738.appspot.com/ 
TEST ENDPOINT https://drogon-flex.appspot.com 





gcloud app deploy app_py37std.yaml -v std-adv-patch-cf 
