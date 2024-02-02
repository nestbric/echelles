<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Echelles statistiques</title>
    <script src="https://d3js.org/d3.v7.min.js"></script>
</head>
<body>
<div id="resultat"></div>

</body>
<script type="module">
    import {posiColor} from './modules/posiColor.js';

    let data, 
        //urlData = "http://localhost/samszo/HDR/docs/assets/data/complexityFrequency.json",
        urlData = "data/fr-en-evaluations_nationales_6eme_region.csv",
        width = 600, height=100, widthLibTxt=100, svg,
        //pVal='cpx',pLib='dim',pFreq='nbCpx',
        pVal='Score moyen',pLib='Matière',pFreq='Ecart type',
        
        interpolates = false;
        /*{
                'Existence':d3.interpolateViridis,
                'Physique':d3.interpolatePlasma,
                'Actant':d3.interpolatePlasma,
                'Concept':d3.interpolatePlasma,
                'Rapport':d3.interpolateYlOrRd
            };
        */
    //d3.json(urlData).then(rs=>{
    d3.csv(urlData).then(rs=>{
        console.log(rs);
        data = setData(rs);
        console.log(data);
        setGraph(data);
    })

    function setData(rs){
        data = Array.from(d3.group(rs, d => d[pLib])).map(d=>{
                    let extX = d3.extent(d[1], d=>d[pVal]),
                        extY = d3.extent(d[1], d=>d[pFreq]),
                        o = {'vals':d[1],
                        'extX':[1,extX[1]],
                        'scX':d3.scaleLinear().domain(extX).range([widthLibTxt, width-widthLibTxt]),
                        'scY':d3.scaleLinear().domain(extY).range([0, height])
                        };
                        o[pLib]=d[0];
                    return o;
                });
        return data;
    }

    function setGraph(data){
        //liste des echelle de couleurs : https://d3js.org/d3-scale-chromatic/sequential
        let pc = new posiColor({'data':data,'cont':d3.select('#resultat')
            , 'pVal':pVal,'pLib':pLib, 'pFreq':pFreq,'frequency':false
            , 'interpolates':interpolates        
        })
    }    

</script>
</html>
