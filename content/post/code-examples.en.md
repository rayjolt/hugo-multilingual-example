+++
date = "2017-03-20T22:30:24"
title = "Code examples"
tags = ["code", "examples"]
categories = ["examples"]
slug = "code-examples"
draft = false

+++

Lorem ipsum dolor sit amet, est quot numquam reformidans te, graeci vivendo dissentiet ut qui. Eam aperiam noluisse persecuti ut, erat tritani elaboraret qui id. Vim tamquam dolores te, quo eu sonet dolore soluta, dicunt veritus periculis pri ex. His error consequuntur et.

PHP code:

``` php
function get_random_bytes($count)
{
        $output = '';
        if (is_readable('/dev/urandom') &&
            ($fh = @fopen('/dev/urandom', 'rb'))) {
                $output = fread($fh, $count);
                fclose($fh);
        }

        if (strlen($output) < $count) {
                $output = '';
                for ($i = 0; $i < $count; $i += 16) {
                        $this->random_state =
                            md5(microtime() . $this->random_state);
                        $output .=
                            pack('H*', md5($this->random_state));
                }
                $output = substr($output, 0, $count);
        }

        return $output;
}
```

Eum partem menandri principes in. His at sumo graecis commune, an facer veritus consetetur est. Cetero vocent comprehensam eu qui, cu quis eleifend contentiones est. Duo idque zril petentium at, ei utinam feugait gloriatur mea. Putent suscipit gloriatur est an, augue electram ut has. Sit in animal delenit, duo facer sanctus debitis in. Ne dictas euismod vis, vide nulla ne sit.

In eos posse vivendum. Vel cu noster utamur delectus, et eius scripta salutatus quo. Autem adipiscing vim ad, an commodo dissentias duo. Sit etiam soluta facete te, labitur moderatius temporibus cu mei. Eos fugit elitr consequuntur no.

C code:

``` c
#include <string.h>
#include <stdarg.h>
#include <stdlib.h>
#include <limits.h>
 
char *concat(const char *s1, ...)
{
	va_list args;
	const char *s;
	char *p, *result;
	size_t l, m, n;
 
	m = n = strlen(s1);
	va_start(args, s1);
	while ((s = va_arg(args, char *))) {
		l = strlen(s);
		if ((m += l) < l) break;
	}
	va_end(args);
	if (s || m >= INT_MAX) return NULL;
 
	result = (char *)malloc(m + 1);
	if (!result) return NULL;
 
	memcpy(p = result, s1, n);
	p += n;
	va_start(args, s1);
	while ((s = va_arg(args, char *))) {
		l = strlen(s);
		if ((n += l) < l || n > m) break;
		memcpy(p, s, l);
		p += l;
	}
	va_end(args);
	if (s || m != n || p != result + n) {
		free(result);
		return NULL;
	}
 
	*p = 0;
	return result;
}
```

Stet saepe postulant vix ea, id nonumes vulputate mnesarchum nec. No legimus laoreet accusata per, ipsum equidem pri ad. Delenit consulatu cotidieque ei duo, pro ea erat sapientem. An nullam dissentiunt quo.

Instructior necessitatibus id sit. Vim hinc exerci et. Eam te stet scaevola comprehensam. Clita verterem persecuti eu duo, nam ad harum putent mediocrem.