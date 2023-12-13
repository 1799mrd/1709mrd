# Выполнение задания для геноаналитики

## Задания данные для выполнения 
Всего было дано 3 задания

- `Задание 1` - Есть:
- заархивированный файл с чтениями (reads.fastq.bz2),
- файл с референсным геномом (genome.fasta).
Надо сначала создать индексы референсного генома для bowtie2. А потом локально откартировать чтения на геном и вывести в терминале какой процент генома имеет покрытие не меньше 10. Желательно не создавать временных файлах на диске (не считая индексов для bowtie2).
 </br>
- `Задание 2` Надо написать bash-скрипт, у которого первым параметром будет некое число, а последующие - произвольное кол-во файлов с расширением txt (столбцы в них разделены запятой).
Скрипт должен выводить 3 столбца, разделенных табуляцией:
- название файла без расширения txt и пути к файлу,
- общее кол-во строк в файле,
- кол-во строк, где значение во втором столбце файла совпадает с первым параметром скрипта.
- `Задание 3` - Есть несколько bam-файлов, которые указываются в качестве параметров скрипта. Они отсортированны и в целом готовы для дальнейшего анализа. И файл генома genome.fasta.
Надо с помощью программы VarScan создать vcf-файлы для каждого бама, в которых будут только снипы без инделов (и отфильтровать по частоте 0.25). Логи VarScan положить рядом с vcf-файлами, такие же названия файлов только с расширением log.
Все образцы в скрипте надо запустить параллельно. А когда досчитается последний, выдать сообщение в терминал, что все посчиталось.</br></br> 
