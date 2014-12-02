#### Sample unsigend Request
https://api.meetup.com/2/events?&sign=true&photo-host=public&group_urlname=gdg-tc&key=yourkey

#### Sample signed request
http://api.meetup.com/2/events?status=upcoming&order=time&limited_events=False&group_urlname=gdg-tc&desc=false&offset=0&photo-host=public&format=json&page=200&fields=&sig_id=9794564&sig=e0ff37957f1e552ccdbbefa8d1ea8b9840e7d3d6

http://api.meetup.com/2/events?status=upcoming&order=time&limited_events=False&group_urlname=gdg-tc&format=json&page=200&fields=&sig_id=9794564&sig=e0ff37957f1e552ccdbbefa8d1ea8b9840e7d3d6&callback=_polymer_jsonp_callback_0