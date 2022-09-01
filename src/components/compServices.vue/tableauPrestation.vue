<template>
    <v-container>
        <h1 id="h1t">lorem</h1>
        <p id="pt">Lorem ipsum dolor sit amet consectetur adipisicing elit. Quibusdam, amet.</p>
    <v-simple-table>
      <template v-slot:default>
        <thead>
          <tr>
            <th class="text-left">
              <h2>Prestations</h2>
            </th>
            <th class="text-left">
              <h2>Prix</h2>
            </th>
          </tr>
        </thead>
        <tbody>
          <tr
            v-for="item in service"
            :key="item.prestation"
          >
            <td>{{ item.prestation }}</td>
            <td>{{ item.prix }}</td>
          </tr>
        </tbody>
      </template>
    </v-simple-table>
</v-container>
  </template>

<script>
    export default {
      data () {
        return {
          service: [
            {
              prestation: 'Taux horaire T1 (petite mecanique)',
              prix: 70+'Є/ttc',
            },
            {
              prestation: 'Taux horaire T2 (grosse méchanique)',
              prix: 85+'Є/ttc',
            },
            {
              prestation: 'Forfait montage de pneus sur jantes tôle toutes tailes (Pose pneumatiques + équilibrages + valves)',
              prix: 15+'Є/ttc',
            },
            {
              prestation: 'Forfait montages de pneus sur jantes alu 13 à 16 pouces (Pose pneumatiques + équilibrages + valves)',
              prix: 15+'Є/ttc',
            },
            {
              prestation: 'Forfait montage de pneus sur jantes alu de 17 à 20 pouces (Pose pneumatique + équilibrages + valves)',
              prix: 20+'Є/ttc',
            },
            {
              prestation: 'Forfait montage de pneus sur jante alu de 20 à 23 pouces (Pose pneumatique + équilibrages + valves)',
              prix: 30+'Є/ttc',
            },
            {
              prestation: 'Forfait réparation de pneu rapide extérieure',
              prix: 15+'Є/ttc',
            },
            {
              prestation: 'Forfait réparation de pneu intérieur avec équilibrage',
              prix: 30+'Є/ttc',
            },
            {
              prestation: "Diagnostic rapide avec l'outil de diagnostic",
              prix: 34.90+'Є/ttc',
            },
            {
              prestation: 'Diagnostic de haute technicité',
              prix: 79 + 'à' + 129 +'Є/ttc',
            },
            {
              prestation: 'Recharge climatisation (Le réseau de climatisation doit être étanche si celui ci comprend une fuite la recharge le pourra être établie.)',
              prix: 69+'Є/ttc',
            },
            {
              prestation: 'Réglage Géométrie simple',
              prix: 69+'Є/ttc',
            },
            {
              prestation: 'Réglage de géométrie complète (Avent + arrière)',
              prix: 100+'Є/ttc',
            },
            {
              prestation: 'Pose de Batterie selon model de véhicule',
              prix: 20 + 'à' + 40 +'Є/ttc',
            },
            {
              prestation: 'Contrôle technique (une vérification sera établie avant le passage au contrôle pour nous assurer du bon passage de celui-ci.)',
              prix: 109.90+'Є/ttc',
            },
          ],
        }
      },
    }
  </script>

  <style lang="scss">
#h1t, #pt{
    color: black;
    text-align: center;
    margin: 1%;
}

  </style>