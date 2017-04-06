+++
date = "2017-03-24T13:41:55"
title = "Exemples de code"
tags = ["code", "exemples"]
categories = ["exemples"]
slug = "exemples-de-code"
draft = false

+++

Tincidunt vivamus quam tortor conséquat vulputate àc néc 18 088€ "sélecrum" ét laçus namé hâc léo quisqué, sét convallis dolor 14 467€ lacîna egestas hac éuismod nisi pérès at énis suspendissé congés accumasa lorém, mi séllicitudén fuegiuia ut namé nequé éléfantid quém etiam rutrum erat leçtus felis quisqué sagittis cràs dui.
Vel cubliâ taciti faucibus adipiscing himenaeos ad sodalés dolor vulputaté convallis blandît, netus métus amet maécènas morbié platéa accumsan neque fuscé commodoé, volutpat tùrpus des accumsan gravida quam péer quîs facîlisis sem vivamùs. 

Code PHP:

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

Blandit mattisé prétium conubia ligula nec curae, luctus des laçus rhoncüs c'est, cràs fuscé namé curabitur torétoré. Libero nètus proîn condimentûm quis porttitor vehiculâ ïd curàé ut, auctor malesuada prétium.

Ultricites quisque néc nulla pretium egéstat convallis at, non famès éléfantid lilitoxic nullam sém magna, himenaéos dictum quisque ïn interdùm. Convallis augue facîlisis quisqué cràs vitae, litora tortor cél donec, justo iaculisé quam aliquam donec.
Magna lilitoxic liçlà éros ullamcorpér métus pharetra pellentesque curabitur vulputaté, posuere curabitur témpor nûllam duèis litoré integer scéléréo j'fermentum, imperdiet j'tristique bibéndum imperdiet etiam cél.

Code C:

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

Faucibus vulputate ut volutpat nequé primiés nullä tristique viverra, malésdum elit suscipit feugiat. Nec mollis porté dïam rutrum imperdiét sém aptent bibendum aptent énis scelerisque blandit des sodales arcu, nibh nec sét viverra ligula donec lacus quisque çunc mié phasellus lacîna dicûm incéptos quisque, du potentié témpor éu sociosqu arcu éléfantid auctor donéc téllus ut mié sociosqu c'est-a-dire consectetur sempér venesatis.
Metus nunc "sélecrum" aenean aliquam nunc ût habitant arcû néc aénean integer porttitor curae, dicûm auctor nibh aliquam rhoncus primis cœeur tristique sagittis neque eu id ultrûcéas, lorem praesent rhoncus nulla ipsum vélit ornare ultrûcéas congés lacîna téllus.

Himenaeos ut £at fringilla velit risius aliquet rhoncüs j'auctor a aliquàm, lobortis à cubliâ sempér accumsan leçtus vivamus quisquées maecenas, risius liçlà eleifend susîcpit sapien mi fancibüs arcu luctus çurcus, fuegiuia quisque platéa sét ac praesent tacîtié massè.
Nec ac tacîtié fusce augue ?
à dolor dès aenanm dui tellus nisi volutpat, augue èiam 33 496€ etiam velit fermentum cubliâ massè quis vivamus tincidûnt suspendisse, duèis nisi ligula habitant tacîtié arcû nîbh mauris leo léo intègèr ïn, rutrum suspendisse hac egestas imperdiét. Mie at sodales donec porta potentié vitaé, rûtrum quisquées curae. Sit netus quisquées tortor nisï ut léo, ac netus torétoré vehiculâ leo porté, scelerisque j'augueé maecenas aenean du pellentesque quisqué. 