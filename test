var http = new XMLHttpRequest();
        var url = '/user/view_docs';
        var params = 'image_id=0';
        http.open('POST', url, true);
        http.setRequestHeader('Content-type', 'application/x-www-form-urlencoded');
        http.onreadystatechange = function() {
            if(http.readyState == 4 && http.status == 200) {
                alert(http.responseText);
            }
        }
        http.send(params);

        http.onreadystatechange = () => {
          if (http.readyState === http.HEADERS_RECEIVED) {
              var cookie = http.getResponseHeader("Set-Cookie");
              alert(cookie);
          }
        }
